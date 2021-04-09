# Audio-Event-Detection

[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
    <h3 align="center">Audio Event Detection using CNN</h3>
    <p align="center">
    project_description
    <br />
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection">View Demo</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Report Bug</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Request Feature</a>
  </p>
</p>


<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li><a href="#about-the-project">About The Project<a></li>
    <li><a href="#Dataset">Dataset</a></li>
    <li><a href="#Model">Model</a></li>
    <li><a href="#Training">Training</a></li>
    <li><a href="#Evaluation">Evaluation</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About The Project

![Demo Video](https://user-images.githubusercontent.com/72017583/114190743-45682100-9969-11eb-9a14-fea8cd43f803.mp4
)

Audio Event Detection is the task of recognizing sound events like trigger words, instrument, etc in an audio recording.

Recognizing sounds events like alarm and glass breaking can be used for surveillance. Environmental sounds events detection can be used for monitoring biodiversity studies.

## Dataset

We collected a total of about 2000 images of people with masks and about 2000 images of people without a mask. For training purposes, 90% images of each class are used and the rest of the images are utilized for testing purposes.

## Model

![image](https://user-images.githubusercontent.com/72017583/114193589-4ea6bd00-996c-11eb-91e5-5ee016285a5e.png)

![image](https://user-images.githubusercontent.com/72017583/114194765-6e8ab080-996d-11eb-84bb-700caacddccb.png)

## Training

The audio files in the given dataset were read using the 22.5KHz Librosa library. We have used 4s sampling time which made the maximum no.  of samples =88200 . For each data, if file size is less, then we have used zero padding . Then we calculated the Short Time Fourier Transform of the given data. After this, we get the spectrogram with size 513X401 of the given audio files. We resampled them to the size 171X 401.Then we used this data as input to our model along with the class labels.



## Evaluation

![image](https://user-images.githubusercontent.com/72017583/114197120-a98de380-996f-11eb-9d9a-24cd60fedf59.png)

![image](https://user-images.githubusercontent.com/72017583/114197429-f5d92380-996f-11eb-94cc-74443dbb09e7.png)


## Contact

E-Mail - adityaverma.ml@gmail.com

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/adityavermaai
