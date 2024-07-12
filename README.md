### Check this tutorial : https://youtu.be/aC13Qna-3cA

### Environment setup to run FLorence-2 on WSL2 (make sure your CUDA is up to date on Windows and WSL):

        nvidia-smi

        Fri Jul 12 17:45:59 2024
        +-----------------------------------------------------------------------------------------+
        | NVIDIA-SMI 555.42.03              Driver Version: 555.85         CUDA Version: 12.5     |
        |-----------------------------------------+------------------------+----------------------+
        | GPU  Name                 Persistence-M | Bus-Id          Disp.A | Volatile Uncorr. ECC |
        | Fan  Temp   Perf          Pwr:Usage/Cap |           Memory-Usage | GPU-Util  Compute M. |
        |                                         |                        |               MIG M. |
        |=========================================+========================+======================|
        |   0  NVIDIA RTX A5000               On  |   00000000:2D:00.0  On |                  Off |
        | 44%   71C    P2            140W /  230W |   24196MiB /  24564MiB |    100%      Default |
        |                                         |                        |                  N/A |
        +-----------------------------------------+------------------------+----------------------+

        +-----------------------------------------------------------------------------------------+
        | Processes:                                                                              |
        |  GPU   GI   CI        PID   Type   Process name                              GPU Memory |
        |        ID   ID                                                               Usage      |
        |=========================================================================================|
        |    0   N/A  N/A        33      G   /Xwayland                                   N/A      |
        +-----------------------------------------------------------------------------------------+
                
        python3 -mvenv venv
        source venv/bin/activate
        pip install wheel
        pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu121        
        pip install transformers timm packaging ninja
        pip install flash_attn
        pip install einops accelerate peft matplotlib


  ##### For Dataset Prepration:  Check data_prep.ipynb 

  ##### For fine tuning florence2 for object detection task:  fine_tuning_florence2.ipynb
  (Fine tuned Trained model is available in model_checkpoints folder)

  ##### For Inference: test.ipynb

  ##### Output image:

![image](https://github.com/AarohiSingla/Florence-2-Fine-tuning/assets/60029146/4a2d0a8d-de45-4bd6-b31a-18a557c3c8a7)


 
  
