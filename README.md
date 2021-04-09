# Audio Event Detection using CNN

[![LinkedIn][linkedin-shield]][linkedin-url]

<p align="center">
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection">View Demo</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Report Bug</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Request Feature</a>
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

![Demo Video](https://imgflip.com/gif/550j7p)

Audio Event Detection is the task of recognizing sound events like trigger words, instrument, etc in an audio recording.

Recognizing sounds events like alarm and glass breaking can be used for surveillance. Environmental sounds events detection can be used for monitoring biodiversity studies.

## Dataset

The dataset was consist of 1761 audio files which was a subset of Urbansound8k dataset. For training purposes, 80% of data was used and the rest 20% of the data was utilized for testing purposes.

The figure below shows the distribution of dataset among all classes.

![dataset distribution pie chart](https://user-images.githubusercontent.com/72017583/114224736-1664a600-998f-11eb-9a31-222bc9796077.JPG)

Figure below shows the total length of all the classes.

Totla length = Sum of all the samples of class.

![dataset total length distribution](https://user-images.githubusercontent.com/72017583/114224931-5b88d800-998f-11eb-9287-be0ca45bc629.JPG)

Figure below shows the total data of every class present in the dataset and how the data is distributed among the number of samples.

![dataset ex vs samples](https://user-images.githubusercontent.com/72017583/114224989-6e031180-998f-11eb-9687-ae86cebcfc34.JPG)


## Procedure

Figure below shows the Block diagram of the procedure followed in this project.

![image](https://user-images.githubusercontent.com/72017583/114215170-e6afa100-9982-11eb-94b4-ec2d3bc6a17d.png)

## Model

Figure below shows the architecture of the model used in this project.

![image](https://user-images.githubusercontent.com/72017583/114194765-6e8ab080-996d-11eb-84bb-700caacddccb.png)

## Training

The audio files in the given dataset were read using the Librosa library at the sampling rate of 22.5KHz. We allowed maximum audio length of 4s at the time of reading files which made the maximum no. of samples present in one file = 88200 . For each file, if file size was less than 88200, then we have used zero padding to make them equal to 88200 samples.

Then we calculated the Short Time Fourier Transform of the given data. After this, we get the spectrogram with size 513X401 of the given audio files. We resampled them to the size 171X 401.Then we used this data as input to our model along with the class labels for training purpose.



## Evaluation

![image](https://user-images.githubusercontent.com/72017583/114197120-a98de380-996f-11eb-9d9a-24cd60fedf59.png)

![image](https://user-images.githubusercontent.com/72017583/114197429-f5d92380-996f-11eb-94cc-74443dbb09e7.png)

## Contact

E-Mail - adityaverma.ml@gmail.com

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
