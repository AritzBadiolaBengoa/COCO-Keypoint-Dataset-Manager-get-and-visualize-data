# Getting and visualizing data from COCO

[COCO](https://cocodataset.org/#keypoints-2017) is one of the most used datasets for different Computer Vision problems: object detection, keypoint detection, panoptic segmentation and DensePose. In this case, we are focused in the challenge of keypoint detection. So, this application has been created to get and vizualize data from COCO easily.

Main Functions:

**- Loading annotations.**

**- Loading images.**

**- Getting and visualizing any sample from the training or validation dataset, including image, bounding box and keypoint set.**

*One "problem" has been detected in the dataset, regarding the bounding box and the keypoints. In some samples, the keypoints are drawn outside of the bounding box area, and this part of the image in which the keypoints are present but is not included in the bounding box, can be very interesting when training or validating the Computer Vision model. To solve this, the following function has been implemented:

*+Increasing the size of the bounding box, if it is possible, to include the part of the image in which any keypoint is located.*

The project has been developed using *Jupyter Notebook* and has been tested in [Python 3.8](https://www.python.org/downloads/release/python-380/). 

## Installation
First of all it is necessary to install [Jupyter Notebook](https://jupyter.org/install). Follow the instructions included in the link depending on the preferences of each one.

Use the requirements.txt file and [pip](https://pip.pypa.io/en/stable/) to install all the required libraries automatically.

```bash
pip install -r .\requirements.txt
```
## Data
*All the necessary data is downloaded using the code*, anyway if it is prefered to download the data from Google Drive (it can take a lot of time from the original sources) or there is any problem when downloading the data using the code, it is provided in the following [Google Drive link](https://drive.google.com/drive/folders/1SOfu3B0ZSVPOwl757eDOS_aN_XCV7GfP?usp=sharing). Include the files and folders as they are organized in the root folder. Extract the Rar files in the root, in "train2017" and "val2017" folders.

## Usage

The code is self-explanatory, and additional comments are included to clarify what tasks are performed and/or why are perfomed.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
Details included in the LICENCE.txt file.
