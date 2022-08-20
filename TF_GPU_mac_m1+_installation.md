Note: Uninstall Anaconda/Anaconda Navigator and other related previously installed version of conda-based installations. Anaconda and Miniforge cannot co-exist together.

- Step1: How to uninstall Anaconda successfully and completely
```
[Remove Anaconda](https://docs.anaconda.com/anaconda/install/uninstall/)
```

- Optional: If brew does not exist in your system then follow this step first otherwise ignore it.
```
[install brew](https://brew.sh/)
```

- Step2: Install miniforge from brew. 
```
brew install miniforge 
```   

- Step3: Use the below commands to ensure that your shell scripts have correct commands to activate conda environment
```
conda init zsh
```
```
conda init bash
```

- Step4: Create an anaconda environment: conda create -n "name of your virtual env"
```
conda create -n tf -y
```

- Step5: Activate the environment: 
```
conda activate tf
```

- Step5: Install Python: You can install your specific version or the latest version
```
conda install python -y
```

- Step6: Installing TensorFlow
    - Install Apple's Tensorflow dependencies
    ```
    conda install -c apple tensorflow-deps -y
    ```
    - Install Tensorflow-metal to install Apple's Metal GPU APIs for TensorFlow 
    ```
    pip install tensorflow-metal
    ```
    - Install Tensorflow for macos to install MacOS arm64 version of TensorFlow
    ```
    pip install tensorflow-macos
    ```