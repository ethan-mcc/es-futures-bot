# es-futures-bot

This requires a multiple gigabytes of .csv I legally cannot redistribute, it costs $65.00.

Designed for trading futures for E-Mini S&P 500 Futures. 

Trained on data from 2008-current, 1 minute interval.

Training time on RTX 3080 > 30 < 45 minutes

## Requirements:
- CUDA GPU >= 10 GB VRAM

## Prerequisites: 
- Docker CE v18+
- Docker Desktop (Running)
- Docker Desktop Settings > Resources > WSL Integration > Enable integration with additional distros (Switch on)
- WSL 2 (Ubuntu) or CentOS 7 or Rocky Linux 8
  (Installed in WSL 2 or Distro)
    - CUDA 11.2/11.4/11.5/11.8 with a compatible NVIDIA driver (https://developer.nvidia.com/cuda-downloads)
    - nvidia-container-toolkit (https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html)

## Installation:
1. Clone the repository:
    ```
    git clone https://github.com/ethan-mcc/es-futures-bot/
    ```
2. Change directory to es-futures-bot:
    ```
    cd es-futures-bot
    ```
4. Allow WSL 2 to use Docker Desktop:
    ```
    sudo chmod 666 /var/run/docker.sock
    ```    
5. Run Docker Compose:
    ```
    docker-compose up 
    ```
6. Access the JupyterLab at:
    ```
    http://127.0.0.1:8888/lab/
    ```
7. Upload the following files:
    - es1.csv
    - First_Rate_Train.ipynb
8. Open `First_Rate_Train` notebook
9. Watch your computer melt in front of you.
