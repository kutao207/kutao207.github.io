---
layout: home
title: home
permalink: /
description: "SHREC 2021 Track: 3D Point Cloud Change Detection for Street Scenes"

# profile:
#   align: right
#   image: prof_pic.jpg
#   address: >
#     <p>555 your office number</p>
#     <p>123 your address street</p>
#     <p>Your City, State 12345</p>

news: true  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

## Task
The rapid development of 3D acquisition devices enables us to collect billions of points in few hours. However, the analysis of the output data is a challenging task, especially in the field of 3D point cloud change detection. 

In this track, we provide large scale 3D point cloud pairs in two different years. Our goal is to detect the changes from multi-temporal point clouds in a complex street environment. We provide manually labelled ground-truth for training and validation. We expect to encourage researchers to try out different methods, including both deep learning and traditional techniques.

## Dataset

The data is provided by Cyclomedia. We choose over ??  manually annotated street-scene 3D point cloud pairs in two different years. The point clouds are recorded by a lidar sensor on a car. Each point cloud pair represents a street scene in two different years and contains a group of changed or unchanged objects. Objects are annotated into 5 meaningful change types and an extra `undefined` class which will not be evaluated. The five meaningful change labels are:

(1) `Nochange` (2) `Change` (3) `Added` (4) `Removed` (5) `Color_change` 

To explain the class labels, suppose we have a point cloud pair of time t1 and t2. Here, ‘Added’ and ‘Removed’ mean an object existed at time t1 but not at t2 and vice versa. ‘Color_change’ refers to cases where change occurs only in color. ‘Change’ refers to cases where an object is there but changed or replaced by a different object.


<!-- ![](assets/image01.png)
 -->
<img src="assets/image01.png" style="display: block; margin-left: auto; margin-right: auto; width: 80%;">

To fit for a learning system, the dataset is split into training and test sets with the ratio 80% and 20%. For both training and test sets, we provide ground-truth semantic labels.

## Download

To obtain the dataset, you must register first:

## Registration

To participate in the track, please send us an email. In it, please confirm your interest in participation and mention your affiliation and possible co-authors. After filling out and submitting this <img src="/assets/word_icon.jpeg" height="18"> [terms of usage document]() to [shrec@cs.uu.nl](mailto:shrec@cs.uu.nl) and [t.ku@uu.nl](mailto:t.ku@uu.nl), you will get the credentials to download the dataset. 

## Submission

From participants, no later than the deadline mentioned in the schedule, we expect results submitted along with a one-page description of the method used to generate them. Results should be presented as a collection of estimated point clouds containing their change labels.

## Evaluation

The main goal of the track is to segment semantic objects out of the street-scene 3D point clouds. For different classes, IoU (Intersection over Union) is one of the main evaluation metrics. For the whole dataset, the unweighted average of IoU (mIoU) of each class and global accuracy are import indicators. We set these three metrics as the main evaluation indicators.

## Timeline

The registration and submission deadlines are in AoE (Anywhere on Earth) timezone.

-	Jan 4, 2021: The dataset is available.

-	Feb 10, 2021: Registration deadline.

-	March 1, 2021: Submission deadline of the results.

-	March 15, 2021: Track submission to SHREC for review.

-	April 15, 2021: First reviews done, first stage decision on acceptance or rejection.

-	May 15, 2021: First revision due.

-	June 15, 2021: Second stage of reviews complete, decision on acceptance or rejection.

-	June 30, 2021: Final version submission.

-	July 5, 2021: Final decision on acceptance or rejection.

-	September, 2021: Publication online in Computers & Graphics journal.


## Expected participants

All experts interested in 3D point cloud change detection are welcome to participate.



<!-- 

Write your biography here. Tell the world about yourself. Link to your favorite [subreddit](http://reddit.com){:target="\_blank"}. You can put a picture in, too. The code is already in, just name your picture `prof_pic.jpg` and put it in the `img/` folder.

Put your address / P.O. box / other info right below your picture. You can also disable any these elements by editing `profile` property of the YAML header of your `_pages/about.md`. Edit `_bibliography/papers.bib` and Jekyll will render your [publications page](/al-folio/publications/) automatically.

Link to your social media connections, too. This theme is set up to use [Font Awesome icons](http://fortawesome.github.io/Font-Awesome/){:target="\_blank"} and [Academicons](https://jpswalsh.github.io/academicons/){:target="\_blank"}, like the ones below. Add your Facebook, Twitter, LinkedIn, Google Scholar, or just disable all of them. -->
