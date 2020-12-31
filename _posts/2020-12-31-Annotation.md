---
layout: post
title:  My way of annotation
---



<!-- <div class="embed-container">
  <iframe
      width="640"
      height="480"
      src="https://drive.google.com/file/d/1_JGPpORRfhVdwEftcHModCPCrjI-Pdb9/view"
      frameborder="0"
      allowfullscreen="">
  </iframe>
</div> -->

<div class="embed-container" align="center">
        <iframe src="https://kutao207.github.io/assets/videos/20-30-28.mp4" width="640" height="360" frameborder="0" allowfullscreen="" allow="autoplay">
        </iframe>
</div>

You can download the video [here](https://kutao207.github.io/assets/videos/20-30-28.mp4).

There are some important steps:

Step 1: **Firstly add a scalar field with point index.** The reason is that after we finish segmenting out different types of change objects, the result are stored in different `txt` files. If we concatenate these files directly, the point order will be different from orginal laz file. We need to merge these files (via an easy python script) to make the points arranged in original order. The point index can be helpful.

**Left click** the `0_WE1NZ71I_2020` file in CloudCompare. `Edit -> Scalar Fields -> Add point indexs as SF` to add point indexs as a column in the file.


<img src="/assets/Screenshot01.png" style="display: block; margin-left: auto; margin-right: auto; width: 100%;">

Step 2: **By using the `Segment Tool` in CloudCompare, we can segment out different types of object.** Please see the operations in the video. (Shortcuts: `space` for start/pause polygonal selection, `left clik`: add contour points, `right click`: finish adding contour points, `i`: segment in the selected area, `o`: segment out the selected area) My keyboard input are all recorded and shown in the lower left side of the video.

Step 3: **After finished labelling, add a scalar field named `type` for each segmented part.** You can define an int number for each type. In the video, `1` denotes `Added`, `2` is `Nochange` and `-1` means `Unfinished`.

<img src="/assets/Screenshot03.png" style="display: block; margin-left: auto; margin-right: auto; width: 100%;">
<img src="/assets/Screenshot04.png" style="display: block; margin-left: auto; margin-right: auto; width: 100%;">

Step 4: **Then, we can save the results to three seperate `txt` files.** It would be easy to merge them and arrange the point in original order by writing a simple python script. You may notice that the `id` and `type` are float numbers which is caused by CloudCompare default setting. It's not a big problem.

<img src="/assets/Screenshot05-1.png" style="display: block; margin-left: auto; margin-right: auto; width: 100%;">
<img src="/assets/Screenshot05-2.png" style="display: block; margin-left: auto; margin-right: auto; width: 100%;">
<img src="/assets/Screenshot05-3.png" style="display: block; margin-left: auto; margin-right: auto; width: 100%;">
