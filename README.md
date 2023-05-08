Download Link: https://assignmentchef.com/product/solved-project-1-of-cse-473-573
<br>
<h1>1           Edge Detection [5 points]</h1>

Figure 1: Image for edge detection

Write programs to detect edges in Fig. 1 (along both <em>x </em>and <em>y </em>directions) using Sobel operator. In your report, please include two resulting images, one showing edges along <em>x </em>direction and the other showing edges along <em>y </em>direction.

<h1>2           Keypoint Detection [5 points]</h1>

Write programs to detect keypoints in an image according to the following steps, which are also the first three steps of Scale-Invariant Feature Transform (SIFT).

<ol>

 <li>Generate four octaves. Each octave is composed of five images blurred using Gaussian kernels. For eachoctave, the bandwidth parameters <em>σ </em>(five different scales) of the Gaussian kernels are shown in Tab. 1.</li>

 <li>Compute Difference of Gaussian (DoG) for all four octaves.</li>

 <li>Detect keypoints which are located at the maxima or minima of the DoG images. You only need to providepixel-level locations of the keypoints; you do not need to provide sub-pixel-level locations.</li>

</ol>

In your report, please (1) include images of the second and third octave and specify their resolution (width × height, unit pixel); (2) include DoG images obtained using the second and third octave; (3) clearly show all the

1

Figure 2: Image for keypoint detection

<table width="235">

 <tbody>

  <tr>

   <td width="56">Octave</td>

   <td width="40"> </td>

   <td width="23"> </td>

   <td width="40">√</td>

   <td width="29"> </td>

   <td width="47">√</td>

  </tr>

  <tr>

   <td width="56">1st</td>

   <td width="40"></td>

   <td width="23">1</td>

   <td width="40">2√</td>

   <td width="29">2</td>

   <td width="47">2 2 √</td>

  </tr>

  <tr>

   <td width="56">2nd</td>

   <td width="40">√2</td>

   <td width="23">2</td>

   <td width="40">2 2 √</td>

   <td width="29">4</td>

   <td width="47">4 2 √</td>

  </tr>

  <tr>

   <td width="56">3rd</td>

   <td width="40">2 2 √</td>

   <td width="23">4</td>

   <td width="40">4 2 √</td>

   <td width="29">8</td>

   <td width="47">8 2 √</td>

  </tr>

  <tr>

   <td width="56">4th</td>

   <td width="40">4 2</td>

   <td width="23">8</td>

   <td width="40">8 2</td>

   <td width="29">16</td>

   <td width="47">16 2</td>

  </tr>

 </tbody>

</table>

Table 1: The bandwidth parameters <em>σ </em>(five different scales) of the Gaussian kernels used in the first step of keypoint detection.

detected keypoints using white dots on the original image (4) provide coordinates of the five left-most detected keypoints (the origin is set to be the top-left corner).

<strong>3       Cursor Detection </strong>[5 points + 3 bonus points]

Figure 3: Illustration of cursor detection task, which aims to locate the cursor highlighted in the red circle.

For the task of cursor detection, which aims to locate the cursor in an image, two sets of images and cursor templates, named as ”Set A” and ”Set B”, will be provided to you. Set A is composed of a total number of 25 images and 1 cursor template. Set A is for task 1., i.e., the basic cursor detection which contributes to 5 points. Set B is composed of a total number of 30 images and 3 different cursor template. Set B is for task 2., i.e., which contributes to 3 bonus points.

<ol>

 <li>Detect cursors in Set A. [5 points]</li>

 <li>Detect cursors in Set B, which is more challenging. [3 bonus points]</li>

</ol>

Note that we will randomly select and run the code you submitted on a set of 20 withheld images to test the performance of your cursor detection programs.

2