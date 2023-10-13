### _**Introduction**_
This project's intention is to create a model for generating funny memes for the image. The model will be trained on the images and their corresponding captions. For every image we have multiple captions from which the model will learn the context of the image.
The project has been picked from - **[GitHub Repo](https://github.com/alpv95/Dank-Learning).** They scraped the data from **[Meme Generator Website](https://memegenerator.net)** which is not active anymore. So we have used the data which they have stored at [Path](https://github.com/alpv95/Dank-Learning/tree/master/im2txt/memes).

### _**Setup**_
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