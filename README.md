# Audio-Event-Detection
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
***
***
***
*** To avoid retyping too much info. Do a search and replace for the following:
*** adityavermaAI, Audio-Event-Detection, twitter_handle, adityaverma.ml@gmail.com, Audio-Event-Detection, project_description
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/adityavermaAI/Audio-Event-Detection">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Audio-Event-Detection</h3>

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

_For more examples, please refer to the [Documentation](https://example.com)_

## Training

The audio files in the given dataset were read using the 22.5KHz Librosa library. We have used 4s sampling time which made the maximum no.  of samples =88200 . For each data, if file size is less, then we have used zero padding . Then we calculated the Short Time Fourier Transform of the given data. After this, we get the spectrogram with size 513X401 of the given audio files. We resampled them to the size 171X 401.Then we used this data as input to our model along with the class labels.



## Evaluation

![image](https://user-images.githubusercontent.com/72017583/114197120-a98de380-996f-11eb-9d9a-24cd60fedf59.png)

![image](https://user-images.githubusercontent.com/72017583/114197429-f5d92380-996f-11eb-94cc-74443dbb09e7.png)


## Contact

E-Mail - adityaverma.ml@gmail.com

LinkedIn: [www.linkedin.com/in/adityavermaai
](www.linkedin.com/in/adityavermaai)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* []()
* []()
* []()





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/adityavermaAI/repo.svg?style=for-the-badge
[contributors-url]: https://github.com/adityavermaAI/repo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/adityavermaAI/repo.svg?style=for-the-badge
[forks-url]: https://github.com/adityavermaAI/repo/network/members
[stars-shield]: https://img.shields.io/github/stars/adityavermaAI/repo.svg?style=for-the-badge
[stars-url]: https://github.com/adityavermaAI/repo/stargazers
[issues-shield]: https://img.shields.io/github/issues/adityavermaAI/repo.svg?style=for-the-badge
[issues-url]: https://github.com/adityavermaAI/repo/issues
[license-shield]: https://img.shields.io/github/license/adityavermaAI/repo.svg?style=for-the-badge
[license-url]: https://github.com/adityavermaAI/repo/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/adityavermaAI
