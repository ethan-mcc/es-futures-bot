# es-futures-bot

This requires a multiple gigabytes of .csv I legally cannot redistribute, it costs $65.00.

Designed for trading futures for E-Mini S&P 500 Futures. 

Trained on data from 2008-current, 1 minute interval.

Training time on RTX 3080 > 30 < 45 minutes

## Requirements:
- CUDA GPU >= 10 GB VRAM

## Prerequisites: 
- CUDA Toolkit
- Docker Desktop

## Installation:
1. Clone the repository:
    ```
    git clone https://github.com/ethan-mcc/es-futures-bot/
    ```
2. Change directory to es-futures-bot:
    ```
    cd es-futures-bot
    ```
3. Run Docker Compose:
    ```
    docker-compose up 
    ```
4. Access the JupyterLab at:
    ```
    http://127.0.0.1:8888/lab/
    ```
5. Upload the following files:
    - es1.csv
    - First_Rate_Train.ipynb
6. Open `First_Rate_Train` notebook
7. Watch your computer melt in front of you.
