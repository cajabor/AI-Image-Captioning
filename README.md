# AI Image Captioning with BLIP

This project automates the process of extracting images from a webpage and generating descriptive captions using the **BLIP (Bootstrapped Language-Image Pretraining)** model. It scrapes images from a given URL, processes them, and outputs captions for each image. It can also caption images in a given local directory.

## Watch a Demo
[Demo](https://drive.google.com/file/d/1mVSp2PCrlqDKlms2IYnqqz5XiuuhhjcL/view?usp=sharing) 

## Technical Challenges Solved
- **Web Scraping & Image Filtering**: Extracting images from webpages while handling different image formats, malformed URLs, and filtering out low-quality images.
- **Image Captioning with BLIP**: Using **Salesforce's BLIP Image Captioning Model** to generate accurate and meaningful descriptions of images.
- **Handling Various Image Sources**: The script processes images from different resolutions, formats, and structures, ensuring robust performance across diverse websites.

## Features
- **Automated Image Scraping**: Extracts and downloads images from a specified webpage.
- **AI-Powered Captioning**: Uses **BLIP** to generate textual descriptions for images.
- **Efficient Filtering**: Skips irrelevant images such as icons, very small images, and unsupported formats.
- **Logs Captions to a File**: Saves the generated captions along with their respective image URLs in `captions.txt`.

## Installation
Ensure you have the required dependencies installed:

```bash
pip3 install virtualenv 
virtualenv my_env # create a virtual environment my_env
source my_env/bin/activate # activate my_env
pip install langchain==0.1.11 gradio==4.44.0 transformers==4.38.2 bs4==0.0.2 requests==2.31.0 torch==2.2.1
