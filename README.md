# Sign Language to Text Conversion

## Abstract

This project is a real-time method utilizing neural networks for fingerspelling based American Sign Language (ASL), addressing the challenge of communication barriers faced by individuals unfamiliar with sign language or lacking access to interpreters. Leveraging convolutional neural networks (CNNs), our approach achieves a 98.00% accuracy in recognizing the 26 letters of the alphabet. Initially, the hand undergoes filtering to enhance feature extraction, followed by classification to predict gesture classes. By incorporating hand position and orientation, we generate training and testing data for CNNs, enabling efficient recognition of human hand gestures from camera images. This method offers a promising solution for bridging communication gaps, empowering individuals to engage with ASL-based communication seamlessly.

## Introduction

American Sign Language (ASL) stands as a vital mode of communication for individuals who are Deaf and Mute (D&M), constituting their primary means of expressing thoughts and interacting with others. As the only disability experienced by D&M individuals pertains to communication, the utilization of spoken languages becomes impractical, rendering sign language indispensable for facilitating meaningful exchanges. Sign language, characterized by its reliance on visual expressions conveyed through hand gestures, serves as a cornerstone of communication within the D&M community. Within this context, gestures play a pivotal role as nonverbal conduits for conveying ideas, emotions, and messages, all comprehended through visual perception.

The essence of sign language lies in its nonverbal communication components, which are understood exclusively through vision. ASL comprises three fundamental components: handshapes, movements, and locations, each contributing to the rich tapestry of expression within the language. Handshapes denote the formation of specific hand configurations, movements encompass the dynamic changes in hand positions and motions, while locations signify the spatial positioning of gestures within the signing space. Together, these components form the intricate grammar and vocabulary of ASL, enabling D&M individuals to articulate nuanced concepts and engage in diverse forms of interaction.

![image](https://github.com/Bhoomika121002/VirtuoThink-Sign2Text-Empowering-Virtual-Intelligence/assets/78655015/386c5586-51d7-4f8d-bd45-05e4ca423a85)


Central to the project's objective is the development of a robust model capable of recognizing Fingerspelling-based hand gestures, a crucial aspect of ASL utilized for spelling out individual letters and forming complete words. By focusing on Fingerspelling, the model aims to address a fundamental aspect of ASL communication, offering a means for D&M individuals to convey precise lexical information efficiently. Through training and implementation, this endeavor seeks to empower D&M individuals by enhancing their ability to express themselves and engage in seamless communication with others, thereby fostering inclusivity and bridging the gap between the D&M community and the broader society.

![image](https://github.com/Bhoomika121002/VirtuoThink-Sign2Text-Empowering-Virtual-Intelligence/assets/78655015/5a9a023e-f818-4244-9c50-d6abfbdee786)

## Problem Statement 

 
Addressing the communication gap for non-sign language users, we aim to develop a real-time system using neural networks to accurately recognize fingerspelling-based American Sign Language (ASL) gestures. The challenge lies in achieving high accuracy in interpreting the diverse hand configurations representing the 26 letters of the alphabet. Our focus is on developing a reliable solution to bridge communication barriers and enhance accessibility for diverse user groups.

## Objectives

To integrate machine learning models to recognize and interpret variations in sign language expressions accurately.

To implement real-time processing capabilities in the system to ensure prompt and accurate interpretation of ASL fingerspelling gestures for seamless communication.

To compile a diverse database of sign language gestures to cover cultural nuances and regional differences.

## Methodology

The system is a vision-based approach. All signs are represented with bare hands and so it eliminates the problem of using any artificial devices for interaction.

Gesture Classification: 
     
   Algorithm Layer 1:
     
1. Apply Gaussian Blur filter and threshold to the frame taken with openCV to get the processed image after feature extraction.
   
2.This processed image is passed to the CNN model for prediction and if a letter is detected for more than 50 frames then the letter is printed and taken into consideration for forming the word.

3.Space between the words is considered using the blank symbol. 

   Algorithm Layer 2:
   
1.We detect various sets of symbols which show similar results on getting detected.

2.We then classify between those sets using classifiers made for those sets only.

Finger Spelling Sentence Formation Implementation:

Whenever the count of a letter detected exceeds a specific value and no other letter is close to it by a threshold, we print the letter and add it to the current string (In our code we kept the value as 50 and difference threshold as 20).
Otherwise, we clear the current dictionary which has the count of detections of the present symbol to avoid the probability of a wrong letter getting predicted.
Whenever the count of a blank (plain background) detected exceeds a specific value and if the current buffer is empty no spaces are detected.
In another case it predicts the end of a word by printing a space and the current gets appended to the sentence below. 

AutoCorrect Feature:

A python library Hunspell_suggest is used to suggest correct alternatives for each (incorrect) input word and we display a set of words matching the current word in which the user can select a word to append it to the current sentence. This helps in reducing mistakes committed in spellings and assists in predicting complex words.


## Conclusion
A real-time vision-based American Sign Language (ASL) recognition system developed for Deaf and Mute (D&M) individuals, focusing on ASL alphabets.

A final accuracy of 98.0% on the dataset, with significant improvement achieved through the implementation of two layers of algorithms.

Enhanced prediction process enables differentiation between symbols with high similarity, improving system accuracy and robustness.

The system demonstrates the capability to detect nearly all ASL symbols under optimal conditions: clear presentation, minimal background noise, and adequate lighting.

The developed ASL recognition system showcases promising accuracy and functionality, offering potential to significantly enhance communication opportunities for the D&M community. Continued advancements in technology and algorithm refinement hold promise for further improving system accuracy and usability, ultimately fostering greater inclusivity and communication access for D&M individuals.








