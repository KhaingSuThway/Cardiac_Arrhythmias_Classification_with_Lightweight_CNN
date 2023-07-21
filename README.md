# Cardiac Arrhythmias (AF,NSR,PAC,PVC) Classification with lightweight CNN

[Optional: Repository Description]

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Usage](#usage)
- [Data Source](#data-source)
- [Preprocessing](#preprocessing)
- [Training](#training)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Welcome to our groundbreaking study! We aim to detect atrial fibrillation (AF) from normal sinus rhythm (NSR) using a lightweight deep learning neural network tailored for mobile devices. By transforming 30-second ECG interval segments into images, we'll classify cardiac arrhythmias, including premature atrial and ventricular contractions (PAC and PVC). PAC is often misdiagnosed and called the "Silent Killer," making its detection crucial.

Our research benefits underserved communities with limited access to cardiology specialists and equipment. By eliminating the need for trained personnel, our system allows for easy detection of abnormal heart rhythms, even in COVID-19 patients needing constant monitoring. Early arrhythmia detection improves treatment outcomes, making our study essential for advancing medical research and enhancing patient care. Together, we can revolutionize healthcare accessibility and transform lives.

## Features


Welcome to our cutting-edge research, where we embark on an exciting journey to detect cardiac arrhythmias using ECG data. Here's a sneak peek into our streamlined and powerful process:

Preprocess ECG Data: We refine raw ECG data, transforming it into images ready for analysis. Noise and artifacts are removed to ensure high-quality data.

Create Datasets: Our data is the backbone of success! We divide it into three subsets: training, validation, and testing. This way, our models get the perfect training, fine-tuning, and a fair shot at proving their worth.

Build Input Pipeline: We've designed an efficient data pipeline that prepares our input for the models. Our data undergoes resizing, normalization, and augmentation to enhance training.

Instantiate Model: Our star player, a carefully chosen model architecture, takes the stage for arrhythmia detection. Rigorous research and testing led us to this perfect match.

Train the Model: Watch the magic unfold as our model learns to recognize and classify different types of arrhythmias. It's like teaching an AI wizard!

Record and Analyze Performance: We meticulously record and analyze our model's performance. We're talking accuracy, sensitivity, and specificity, among others. It's like detective work with AI flair!

Iterate with Alternative Models: We don't stop at just one model. No siree! We love exploring new avenues and trying out alternative architectures. It's like a thrilling adventure through a maze of possibilities.

Compare and Conclude Results: We gather our findings, meticulously compare the models, and draw meaningful conclusions. Our goal is to uncover the most effective approach for arrhythmia detection, guiding future research directions.

This research is about making a real impact on medical care, especially for those who need it most. We're determined to revolutionize the way we detect arrhythmias, and we can't wait to share our breakthroughs with the world. So, buckle up for an exhilarating ride into the future of healthcare! Stay tuned for more exciting updates from the forefront of technology and medicine.

## Requirements

The 'requirements.txt' file lists all the essential dependencies needed to run our project smoothly. With just a simple command, you'll be all set to explore the fascinating world of cardiac arrhythmia detection. No more hassle of figuring out which libraries to install or worrying about compatibility issues. 

## Long-Term Atrial Fibrillation (LTAF) database

It's like a treasure trove of ECG data regarding to Atrial Fibrillation, collected from physionet.org, with 84 records of around 24-hour long ECG recordings, all with a sampling frequency of 128 Hz. Serious data power, right? 📊🔥
And that's not all - the icing on the cake is that each of these records comes with annotations for beat and rhythm type.These labels are pure gold, making our algorithm development and testing a breeze. Let's toast to smooth data analysis! 🎉🥂
Big shoutout to the brilliant minds at PhysioNet for hooking us up with their user-friendly wfdb Python library. It's like a magic wand for accessing, analyzing, and manipulating physiological signals. We're crushing it! 🪄💻

Now, let's dive into the juicy details. The LTAF database treats us to five types of beat annotations: N for Normal Sinus Rhythm, A for premature atrial contraction, V for premature ventricular contraction, Q for unknown beat, and ' " ' for missing beat. On the rhythm side, we've got nine types of annotations to play with. For this one, we're zooming in on the heart-stealers - atrial fibrillation and normal sinus rhythm for rhythm-based annotation, and normal beat, premature atrial contraction, and premature ventricular contraction for beat-wise annotation. Let's feel that rhythm! 🎶💓

With this goldmine of annotated data, we're all set to revolutionize cardiac arrhythmia detection! Get ready for some incredible discoveries as we dive deep into the world of heart rhythms. Stay tuned for more thrilling updates, and let's ace the game of arrhythmia analysis together! 💪🔍

## Data Source

[Provide information about the data source you used, including the link to the Long Term Atrial Fibrillation database on PhysioNet.]

## Preprocessing

[Explain the steps involved in reading the ECG records and how they are converted to 30-second records for each of the four arrhythmias. Include the criteria used for the conversion.]

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

[Optionally, you can include an acknowledgments section to credit any external libraries, contributors, or sources that have been instrumental in your project.]


