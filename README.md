# Yolov8 installation guide for python<br/>
1. Create venv for the project directory for package management.<br/><br/>
2. Install ultralytics using pip. <br/>
   ```pip install ultralytics```<br/><br/>
3. Install CUDA version based on the latest one for pytorch.<br/>
   https://developer.nvidia.com/cuda-12-4-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local<br/><br/>
4. Install pytorch from https://pytorch.org/get-started/locally/
   ![image](https://github.com/user-attachments/assets/a126c50c-dca9-4b8c-823d-c22d61af7f41)<br/>
  ```pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124```<br/><br/>
6. Run this command in CLI to test if pytorch successfully installed. (still inside the venv of the project)<br/>
   ```python```<br/>
   ```import torch```<br/>
   ```torch.cuda.is_available()```<br/><br/>
**NOTE**: Incase of WinError 126  caused by pytorch, follow this solution from https://github.com/pytorch/pytorch/issues/131662#issuecomment-2252589253<br/>
   ![image](https://github.com/user-attachments/assets/7cf31b8a-3798-4f84-b5ec-f997de25660d)<br/><br/>

7. Run this command in CLI to test if ultralytics yolov8 is successfully installed. (still inside the venv of the project)<br/>
   ```yolo train data=coco8.yaml model=yolov8n.pt epochs=10 lr0=0.01```<br/>
   ![image](https://github.com/user-attachments/assets/1624c303-33eb-404e-9bda-d6e826415662)<br/>
   Should be able to get this output.
   ![image](https://github.com/user-attachments/assets/e2e31856-4016-4f0b-8763-e20e8b4e5f18)<br/><br/>


## view this video for python and cli guide<br/>
https://www.youtube.com/watch?time_continue=278&v=GsXGnb-A4Kc&embeds_referring_euri=https%3A%2F%2Fdocs.ultralytics.com%2F&source_ve_path=Mjg2NjY

## references<br/>
https://github.com/ultralytics/ultralytics<br/>
https://docs.ultralytics.com/quickstart/#use-ultralytics-with-cli
