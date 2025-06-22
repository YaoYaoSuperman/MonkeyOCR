🚀 Running MonkeyOCR with Transformer as the backend on Mac



This guide will walk you through running MonkeyOCR with Transformer as the backend on your Mac device. Let's get started! 🌟


1\. 🛠️ Preparation



Ensure that your Mac has a Python environment installed.  If not installed, you can install it via Homebrew. Open the terminal and run the following commands:




```
/bin/bash -c "\$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install python
```

Also, make sure you have Anaconda or Miniconda installed. If not, you can install Miniconda via Homebrew:




```
brew install miniconda
```

2\. 📦 Create and Configure the Virtual Environment





**🧪 Create a virtual environment**: Open the terminal and run the following command to create a virtual environment named MonkeyOCR with Python 3.8.




```
conda create -n MonkeyOCR python=3.10
```



**🔋 Activate the virtual environment**:


*   In the bash or zsh terminal of macOS, run:




```
conda activate MonkeyOCR
```

3\. 📥 Install Dependencies





**📦 Install PyTorch and related libraries**: In the activated virtual environment, run the following command to install the specified versions of PyTorch, torchvision, and torchaudio.




```
pip install torch==2.5.1 torchvision==0.20.1 torchaudio==2.5.1
```



**🔧 Install project dependencies**: Navigate to the directory where the MonkeyOCR project is located and run the following command to install the project dependencies.




```
pip install -e .
```

4\.🚀 Run MonkeyOCR



After completing the above steps, run the following command to perform OCR recognition on the sample image:




```
python parse.py ./demo/demo.png
```

📊 Performance Reference



On an M4 AIR with 16GB of RAM, when `bs = 2` is set, the measured running time is 341.62 seconds. You can adjust the parameters according to your device's performance to optimize the running efficiency.


The above are the complete steps for running MonkeyOCR on Mac. If you encounter any problems during the running process, you can check whether the environment configuration or modification steps are correct. Feel free to let me know the details of the problems. 😊

