# Remove-Background-Bulk-Image-Video

Python to remove background and adding new background image

- Remove background from **images,videos & live webcam**
- Adding new background to those **images,videos & webcam footage**

### Demo

<table>
<tr align="center">
<td><b>Before removing the background</b></td>
<td><b>After removing the background</b></td>
</tr>
<tr align="center">
<td><img src="assets/image/11.jpg" alt="decoration.jpg" width="460" height="500"/></td>
<td><img src="output/11.png" alt="decoration.png" width="460" height="500"/></td>
</tr>
<tr align="center">
<td><b>Before removing the background</b></td>
<td><b>After replacing the background with new image</b></td>
</tr>
<tr align="center">
<td><img src="assets/image/13.jpg" alt="mukut.jpg" width="460" height="500"/></td>
<td><img src="output/13.png" alt="mukut.png" width="460" height="500"/></td>
</tr>

<table>

## Installation

### Python Version

- Python == 3.8

### Virtual Environment

#### Windows

- `python -m venv venv`
- `.\venv\Scripts\activate`
- If any problem for scripts activation
  - Execute following command in administration mode
    - `Set-ExecutionPolicy Unrestricted -Force`
  - Later you can revert the change
    - `Set-ExecutionPolicy restricted -Force`

#### Linux

- `python -m venv venv`
- `source venv/bin/activate`

### Library Installation

- Library Install
  - `pip install --upgrade pip`
  - `pip install --upgrade setuptools`
  - `pip install -r requirements.txt`


## Remove

### Image

#### Single image

It will generate the output file in **output/** folder

- `python inference.py --image image_path` **[Without background image]**
- `python inference.py --image image_path --background True` **[With background image]**
- Example:
  - `python inference.py --image assets/sample_image/female.jpeg`
  - `python inference.py --image assets/sample_image/male.jpeg --background True`

#### Folder of images

It will generate the output file in **output/** folder

- `python inference.py --folder folder_path` **[Without background image]**
- `python inference.py --folder folder_path --background True` **[With background image]**
- Example:
  - `python inference.py --folder assets/sample_image/`
  - `python inference.py --folder assets/sample_image/ --background True`

### Video

It will generate the output file in **output/** folder

- `python inference.py --video video_path` **[Without background image]**
- `python inference.py --video video_path --background True` **[With background image]**
- Example:
  - `python inference.py --video assets/sample_video/sample.mp4`
  - `python inference.py --video assets/sample_video/sample.mp4 --background True`

### Webcam

- `python inference.py --webcam True` **[Without background image]**
- `python inference.py --webcam True --background True` **[With background image]**

