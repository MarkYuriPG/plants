# Yolov8 installation guide for python

1. Create venv for the project directory for package management.
2. Install ultralytics using pip.
   ```pip install ultralytics```
3. Install CUDA version based on the latest one for pytorch.
   https://developer.nvidia.com/cuda-12-4-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local
4. Install pytorch from https://pytorch.org/get-started/locally/
   ![image](https://github.com/user-attachments/assets/a126c50c-dca9-4b8c-823d-c22d61af7f41)
  ```pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124```
5. Run this command in CLI to test if pytorch successfully installed. (still inside the venv of the project)
   ```python```
   ```import torch```
   ```torch.cuda.is_available()```
6. Run this command in CLI to test if ultralytics yolov8 is successfully installed. (still inside the venv of the project)
   ```yolo train data=coco8.yaml model=yolov8n.pt epochs=10 lr0=0.01```
   ![image](https://github.com/user-attachments/assets/1624c303-33eb-404e-9bda-d6e826415662)
7. Hurray!

##view this video for python and cli guide
https://www.youtube.com/watch?time_continue=278&v=GsXGnb-A4Kc&embeds_referring_euri=https%3A%2F%2Fdocs.ultralytics.com%2F&source_ve_path=Mjg2NjY

## references:
https://github.com/ultralytics/ultralytics
https://docs.ultralytics.com/quickstart/#use-ultralytics-with-cli
