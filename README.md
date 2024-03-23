# Cardiac Arrhythmias (AF,NSR,PAC,PVC) Classification with lightweight CNN

You can find the paper at this link:
[Cardiac Arrhythmia Detection Paper](https://ieeexplore.ieee.org/abstract/document/9894861). 
If you find our research helpful, we kindly request you to cite our paper

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Data Source](#data-source)
- [Preprocessing](#preprocessing)
- [Training](#training)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Get ready to dive into a groundbreaking study that will blow your mind - we're all about detecting cardiac arrhythmias with a lightweight deep learning neural network!  Our mission is crystal clear: we want to detect atrial fibrillation (AF) from normal sinus rhythm (NSR) using a neural network that's perfect for mobile devices with limited computational resources. Say goodbye to complexity and hello to efficiency! 

Picture this: 30-second ECG interval segments as our secret weapon for classification. Clinically recognized AF episodes last at least 30 seconds, so we've got the perfect timeframe for the job. Plus, we're transforming these segments into images - it's like a creative ECG art project!  But wait, there's more! We're not stopping at AF detection. We've got a whole squad of arrhythmias to classify, including premature atrial and ventricular contractions (PAC and PVC). These sneaky conditions can lead to AF gradually, and PAC is known as the "Silent Killer" - so we're on a mission to expose them! 

Our study has got a heart of gold. We're here to make a real difference for those living in rural areas, where access to cardiology specialists and monitoring equipment is limited. With our lightweight neural network and portable ECG access, detecting abnormal heart rhythms becomes a breeze - even for COVID-19 patients requiring constant monitoring. The future of healthcare is looking brighter already! Early arrhythmia detection means better treatment outcomes and enhanced options for doctors. We're talking about a whole new level of patient care and medical research advancement! 

Join us on this epic journey as we revolutionize arrhythmia detection using cutting-edge technology. Our impact is going to be huge, especially for underserved communities lacking advanced healthcare. We're all about making lives better and leaving no one behind. Let's embark on this exciting adventure together! 

## Features

Get ready to witness the power of our cutting-edge research procedure for cardiac arrhythmia detection!

Preprocess ECG Data: We work behind the scenes to refine raw ECG data, transforming it into crystal-clear images ready for analysis. Say goodbye to noise and artifacts - we're all about high-quality data! 

Create Datasets: Our data game is strong! We divide it into three subsets: training, validation, and testing. This means our models get the VIP treatment, from training to fine-tuning and evaluation. Talk about fairness! 

Build Input Pipeline: Our data pipeline is smooth like butter! We've designed it to effortlessly prepare data for the models. From resizing to normalization and cool augmentation techniques - we've got it all covered. No more data headaches! 

Instantiate Model: Our star player, a hand-picked model architecture, takes center stage for arrhythmia detection. Thanks to rigorous research and testing, we've got the perfect match. It's all about that perfect chemistry! 

Train the Model: Brace yourself for the magic show! Our model learns to recognize and classify different types of arrhythmias like a pro. 

Record and Analyze Performance: We're all about the numbers game! We meticulously record and analyze our model's performance. Accuracy, sensitivity, specificity - you name it, we've got it. 

Iterate with Alternative Models: One model is not enough for us! We're explorers at heart. So we try out different architectures, like going on a thrilling adventure through the world of AI possibilities. Compare and Conclude Results: The ultimate showdown! We compare models and draw meaningful conclusions. 

Our research procedure is like a well-choreographed dance, making cardiac arrhythmia detection a breeze. It's all about efficiency, accuracy, and groundbreaking discoveries. 
## Requirements

The 'requirements.txt' file lists all the essential dependencies needed to run our project smoothly. With just a simple command, you'll be all set to explore the fascinating world of cardiac arrhythmia detection. No more hassle of figuring out which libraries to install or worrying about compatibility issues. 

## Data Source
#### Long-Term Atrial Fibrillation (LTAF) database

It's like a treasure trove of ECG data regarding to Atrial Fibrillation, collected from physionet.org, with 84 records of around 24-hour long ECG recordings, all with a sampling frequency of 128 Hz. Each of these records comes with annotations for beat and rhythm type.These labels are pure gold, making our algorithm development and testing a breeze. Let's toast to smooth data analysis!
PhysioNet for hooking us up with their user-friendly wfdb Python library. The LTAF database treats us to five types of beat annotations: N for Normal Sinus Rhythm, A for premature atrial contraction, V for premature ventricular contraction, Q for unknown beat, and ' " ' for missing beat. On the rhythm side, we've got nine types of annotations to play with. For this one, we're zooming in on the heart-stealers - atrial fibrillation and normal sinus rhythm for rhythm-based annotation, and normal beat, premature atrial contraction, and premature ventricular contraction for beat-wise annotation.

## Preprocessing

We're taking raw ECG signals and turning them into something more useable. It all starts with noise filtering. Those pesky interferences like powerline interferences, baseline wanders, and electromyographic noises are no match for us. We use a 5th order high-pass Butterworth filter with a cutoff frequency of 0.5 Hz to kick baseline wander to the curb. And the 60 Hz powerline interference? We say "bye-bye" to that with a band stop filter centered at 60 Hz.
Once we've got our pristine signals, it's time for data transformation. From the detected QRS complexes, we create individual beats within the 30-second segment are plotted on a clean white background, overlaying those plotted beat images to form a single synchronized beat image. With this image transformation, the difference between arrhythmias and NSR becomes crystal clear. Regular NSR beats show noticeable P, Q, R, S, and T waves.

## Training

[Describe the process of transforming the values from the previous step into ECG beat images and how these images are used to train the lightweight deep learning neural network.]

## Results

[If you have achieved any significant results or milestones, describe them here. Include any performance metrics or visualizations to demonstrate the effectiveness of your approach.]

## Contributing

[Explain how others can contribute to your project. Provide guidelines for submitting issues, feature requests, and pull requests.]

## License

[Specify the license under which your project is distributed. Choose an open-source license that aligns with your preferences.]

[Add any additional sections that you think are necessary or relevant to your project.]

## Acknowledgments

We extend our heartfelt gratitude to the Faculty of Electrical Engineering Department and the Research Council of Biomedical Engineering Program at Chulalongkorn University for their invaluable support and collaboration in this research scholarship. Their contribution has been instrumental in making this study a reality. Thank you for being an essential part of our journey to revolutionize cardiac arrhythmia detection! 🙏🌟


