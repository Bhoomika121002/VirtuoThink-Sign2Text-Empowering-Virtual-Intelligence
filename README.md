# Sign Language to Text Conversion

## Abstract

This project is a real-time method utilizing neural networks for fingerspelling based American Sign Language (ASL), addressing the challenge of communication barriers faced by individuals unfamiliar with sign language or lacking access to interpreters. Leveraging convolutional neural networks (CNNs), our approach achieves a 98.00% accuracy in recognizing the 26 letters of the alphabet. Initially, the hand undergoes filtering to enhance feature extraction, followed by classification to predict gesture classes. By incorporating hand position and orientation, we generate training and testing data for CNNs, enabling efficient recognition of human hand gestures from camera images. This method offers a promising solution for bridging communication gaps, empowering individuals to engage with ASL-based communication seamlessly.

## Libraries Requirements

Note : Python 3.8 or above is required to build this project, as some of the libraries required can't be installed on the lastest version of the Python  

```bash
1. Lastest pip -> pip install --upgrade pip

2. numpy -> pip install numpy

3. string -> pip install strings

4. os-sys -> pip install os-sys

5. opencv -> pip install opencv-python

6. tensorFlow -> i) pip install tensorflow 
                 ii) pip3 install --upgrade https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.8.0-cp34-cp34m-linux_x86_64.whl

7. keras -> pip install keras

8. tkinter -> pip install tk

9. PIL -> pip install Pillow

10. enchant -> pip install pyenchant (Python bindings for the Enchant spellchecking system)

11. hunspell -> pip install cyhunspell (A wrapper on hunspell for use in Python)
```

## Running the Project 

``` python
python /path/to/the/Application.py
```
  
