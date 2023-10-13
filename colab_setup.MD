This Python document covers the steps required to modify the preprocessing.ipynb document to run in Google Colab. This file assumes the following file path to the meme-generation folder in MyDrive: MyDrive/meme-generation <br>
```
from google.colab import drive
drive.mount('/content/drive')

```<br>

Run this above code block before the instantiation of the PROJECT_DIR variable <br>

```
PROJECT_DIR = os.getcwd()  # get the current working directory
DATA_DIR = os.path.join(PROJECT_DIR, 'drive/MyDrive/meme-generation/data') # Concatenate the folder name which contains images
DATA_DIR  # Check the final path value
```

Replace the PROJECT_DIR code block to contain the above code. 
