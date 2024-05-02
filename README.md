# Sign Language to Text Conversion

## Abstract

Sign language is one of the oldest and most natural form of language for communication, but since most people do not know sign language and interpreters are very difficult to come by we have come up with a real time method using neural networks for fingerspelling based american sign language.
 
In this method, the hand is first passed through a filter and after the filter is applied the hand is passed through a classifier which predicts the class of the hand gestures. This method provides 98.00 % accuracy for the 26 letters of the alphabet.

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
  
