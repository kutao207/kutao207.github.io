---
layout: shrec2020
title: shrec2020
permalink: /shrec2020
---

<!-- # SHREC 2020 Track: 3D Point Cloud Semantic Segmentation for Street Scenes -->

## Motivation & Task

Scene understanding of large-scale 3D models of an outer space is still a challenging task. With the development of computer vision techniques, it’s cost-effective to develop a solution for large-scale 3D scenes related tasks, e.g. semantic segmentation for 3D street scenes. 

In this track, we provide large scale 3D point clouds for street scenes. Our goal is to localize and segment semantic objects from large-scale street scene 3D point clouds. We also provide manually labelled ground-truth for training and validation. We expect to encourage researchers to try out different methods, including both deep learning and traditional machine learning techniques.

## Dataset

The data is provided by cyclomedia. We choose 80 3D point clouds for street scenes from the data and manually labelled them. The point clouds are recorded by a lidar sensor on a car. Each point cloud represents a street scene and contains a group of objects. We use the open source software [Cloud Compare](http://cloudcompare.org/) to manually label point clouds. Objects are labelled into 5 meaningful classes and an extra `undefined` class. They are:

(1) `Building` (2) `Car` (3) `Ground` (4) `Pole` (5) `Vegetation` (6) `Undefined`

An example visualization of the sample `5D4KVPBP` is:

<img src="/assets/5D4KVPBP.PNG" style="display: block; margin-left: auto; margin-right: auto; width: 80%;">

To fit for a learning system, the dataset is split into training with 60 samples and test sets with 20 samples. For both training and test sets, we provide ground-truth semantic labels.

**To obtain the data set you must register first:**

## Download

**The dataset is now publicly available [here](https://drive.google.com/drive/folders/1kJPps7R9gr6vt098nzGsooOBVKKA5969?usp=sharing).**

## Registration

To participate in the track, please send us an email. In it, please confirm your interest in participation and mention your affiliation and possible co-authors. After filling out and submitting this <img src="/assets/word_icon.jpeg" height="18"> [terms of usage document](/assets/SHREC2020%20Terms%20of%20Use%20of%20CMT%20UU%20%20data.docx) to [shrec@cs.uu.nl](mailto:shrec@cs.uu.nl) and [t.ku@uu.nl](mailto:t.ku@uu.nl), you will get the credentials to download the data set. 

## Submission

From participants, no later than the deadline mentioned in the schedule, we expect results submitted along with a one-page description of the method used to generate them. Results for test data set should be presented as a collection of estimated point clouds containing their semantic labels. To reduce the result file size, you can only submit semantic labels of each point cloud in separate files.

## Evaluation

The main goal of the track is to segment semantic objects out of the street-scene 3D point clouds. For different classes, IoU (Intersection over Union) is one of the main evaluation metrics. For the whole dataset, the unweighted average of IoU (mIoU) of each class and global accuracy are import indicators. We set these three metrics as the main evaluation indicators.

## Organizers

- Tao Ku, Utrecht University, Department of Information and Computing Sciences
- Remco C. Veltkamp, Utrecht University, Department of Information and Computing Sciences
- Bas Boom, Cyclomedia Technology

To contact the organizers, please contact [t.ku@uu.nl](mailto:t.ku@uu.nl)

## Schedule

The registration and submission deadlines are in AoE (Anywhere on Earth) timezone.

- March 2, 2020: The dataset is available.
- ~~March 15~~ April 5, 2020: Registration deadline.
- ~~March~~ **April 18, 2020: Submission deadline of the results.**
- ~~April 3~~ May 3, 2020: Track submission to SHREC for review.
- ~~May~~ June 1, 2020: Reviews done, first stage decision on acceptance or rejection
- ~~May~~ June 22, 2020: First revision.
- ~~May~~ June 29, 2020: Second stage decision on acceptance or rejection.
- ~~June~~ July 12, 2020: First revision.
- ~~June~~ July 19, 2020: Final decision on acceptance or rejection.
- September 1, 2020: Publication online in Computers & Graphics.
- September 4-5, 2020: Eurographics Workshop on 3D Object Retrieval 2020, featuring SHREC 2020.

## References

1.	Zolanvari, S. M., Ruano, S., Rana, A., Cummins, A., Silva, R. E., Rahbar, M., & Smolic, A. (2019). DublinCity: Annotated LiDAR Point Cloud and its Applications. arXiv: Computer Vision and Pattern Recognition.


<br/>
<br/>

<img src="/assets/logo_cyclomedia.jpg" width="150">

> CycloMedia develops, builds and operates the worlds most advanced mobile mapping systems. With a combination of sensors ranging from cameras and Lidar scanners to state-of-the-art positioning systems we map dense urban areas in Western Europe and North America. Point clouds and images are accurately geo-registered, where the panoramic imagery is of high geometric quality.
> The petabytes of data (all processed and stored in the Microsoft Azure cloud) that we collect every year are used by “professional users”, ranging from city governments to large corporates working in utilities, infrastructure and insurance. Their one common denominator is their need for better data and information to drive change in how they can serve their inhabitants and customers. Today our solutions make cities more safe, green, accessible and smart and help companies to make the right decisions based on fresh and accurate data. CycloMedia is based in The Netherlands and has offices in the US and Germany.

