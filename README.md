# **<p align="center">Meme Generation</p>**

## _**Introduction**_
This project's intention is to create a model for generating funny memes for the image. The model will be trained on the images and their corresponding captions. For every image we have multiple captions from which the model will learn the context of the image.
The project has been picked from - **[GitHub Repo](https://github.com/alpv95/Dank-Learning).** They scraped the data from **[Meme Generator Website](https://memegenerator.net)** which is not active anymore. So we have used the data which they have stored at [Path](https://github.com/alpv95/Dank-Learning/tree/master/im2txt/memes).

## _**Setup**_

### **Cloning the Repository with Large Files (Using Git LFS)**
<u> **Prerequisites**</u><br>
Before cloning the repository, ensure that you have the following prerequisites installed:
1. <u>Git</u>: You need Git installed to clone the repository. If you don't have Git installed, download and install it from [Git's official site](https://git-scm.com/downloads).

2. <u>Git LFS</u>: Since this repository uses Git Large File Storage (LFS) for managing large files, Git LFS must be installed on your system. You can download it from [Git LFS's official site](https://git-lfs.com/).

<u> **Cloning the Repository**</u><br>
1. Clone the Repository using command:
    ```
    git clone <repository-url>
    ```
2. Initialize Git LFS:   
    Either <u>globally</u>
    ```
    git lfs install
    ```
    OR <u>local</u> to the specific repository
    ```
    cd <repository-name>
    git lfs install --local
    ```
    When the repository is cloned you would see the `.best.pth` files, but the size would be in KB which indicates that the large file contents are not downloaded. To download the contents perform step 3.

3. Pull the LFS Files:<br>
    To download the large files stored with LFS, use:
    ```
    git lfs pull
    ```

### **Seamless Installation of Libraries**
To have a seamless installation of libraries and proper installation of the cudatoolkit & cudnn, use the conda environment in VS Code. 
1. Install the [miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html) 
2. Create a conda virtual environment and initialize it in VS Code using commands -<br>
    a. ```
        conda create --name venv python=3.10
        ```<br>
    b. ```
        conda init cmd.exe
        ```    
3. Activate the virtual environment
    ```
    conda activate venv
    ```
4. Install the cudatoolkit and cudnn using conda
    ```
    conda install cudatoolkit cudnn
    ```
5. Install the other required libraries using requirements.txt file
    ```
    pip install -r requirements.txt
    ```

## _**Meme Generated by Model**_
The meme generated on 2 unseen images - <br>

![Alt text](Model-Generated-Memes/meme1.png?raw=true "Meme Image1")

![Alt text](Model-Generated-Memes/meme2.png?raw=true "Meme Image2")