# PDF Dark Mode

## About 

### [Pypi page](https://pypi.org/project/PdfDarkMode/)

### _*NOTE:*_ This project is going under significant changes! Stay tuned for updates!

#### This is a python program that converts the white-space in PDF files to have a grey background.
#### This program works best with non-handwritten PDF's and PDF's without any images.

## Installation 
### Windows
- #### Download [poppler for Windows from here.](https://github.com/oschwartz10612/poppler-windows/releases/tag/v20.12.1-data)
- #### Extract the folder somewhere on your PC. 
- #### Add the path C:\<path-to-extracted-folder>\poppler-20.12.1\Library\bin in the Windows Environment PATH. 

### macOS
* #### Mac users will have to install poppler for Mac. You can do so with this [homebrew formula.](https://formulae.brew.sh/formula/poppler)

### Linux
* #### Most distributions of linux already have ```pdftoppm``` installed. If not you can check your package manager on how to install ```poppler-utils```.

### Then
### _*Using pip*_
* #### ``` pip install PdfDarkMode ```
### _*Or*_
* #### ``` git clone https://github.com/JustinTheWhale/PDF-Dark-Mode.git ```
* #### ``` cd PDF-Dark-Mode ```
* #### ``` pip install -r requirements.txt ```


##Usage

```python
from PdfDarkMode.darkmode import convert

convert("example.pdf")
```

#### Additionally, you can pass a list of PDF files instead of just one string like so: 

```python

from PdfDarkMode.darkmode import convert

convert(["example.pdf", "example2.pdf", ...])
```

#### If you dont feel like importing the package (or just didn't install it with pip), you can run it directly from the command line:

```python darkmode.py example.pdf example2.pdf ...```

## Example
<img src="examples/example_input.png">
<img src="examples/example_output.png">