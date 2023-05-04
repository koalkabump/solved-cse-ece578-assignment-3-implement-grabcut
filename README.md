Download Link: https://assignmentchef.com/product/solved-cse-ece578-assignment-3-implement-grabcut
<br>
<strong>Instructions:</strong>

<ul>

 <li>The assignment can be implemented in Python or C++.</li>

 <li><strong>Make sure that the assignment that you submit is your own work. Any breach of this rule could result in serious actions including an F grade in the course.</strong></li>

 <li><strong>This is a fairly large assignment. The experiments and report writing will take time. Start your work early and do not wait till the deadline.</strong></li>

 <li><strong>Write modular code, with comments clearly outlining the function of each module</strong></li>

 <li><strong>Demonstrate the results on the given images and additional images from your camera</strong></li>

 <li>Make sure your files can be opened. Corrupted files will not be entertained.</li>

 <li>The code must be robust and scalable and it should work for images of any size.</li>

 <li>The submission must have a directory called code/ which contains all the code use to generate the results. The report and the output images should be in the report/ directory.</li>

 <li>Please ensure that the report contains your roll number. Zip the assignment folder. The zip file should be named Roll Number assignment3.zip</li>

 <li>Please post your doubts on the Moodle forum instead of asking the TA’s personally.</li>

 <li>There are some sample images included in the assignment, these images are NOT the exhaustive test set. Your code may be tested on a different set.</li>

 <li>Add the procedure and the images of intermediate steps in the report. Add the code to the report as well and explain it wherever necessary.</li>

 <li>Make sure you provide the code separately also and not just in the report.</li>

</ul>

<strong>Tasks:</strong>

<h1>GrabCut</h1>

<ol>

 <li>Implement GrabCut. See Rother et al. for a detailed description of the algorithm.</li>

 <li>Refer to Sec.2 of the Rother paper and Boykov Jolly for details of energy minimization based image segmentation.</li>

 <li><strong>What you need to implement: </strong>You only need to implement the iterative procedure described in Sec.3.1 and Sec.3.2 of the Rother paper to get a binary segmentation of the image. The user interaction interface in Sec.3.3 is optional. You do not need to implement border matting or foreground estimation in Sec.4.</li>

 <li>You can use GMM of standard libraries (sklearn etc) that would be required for implementation of Sec.3.1</li>

 <li>We would be providing you with the test images and bounding boxes. Each image contains only one foreground object and has a corresponding bounding box, which is a rectangle around that object. Please find the images and bounding boxes</li>

 <li>The final program must have a GUI component that allows the user to draw the bounding box which specifies the foreground object in an image and the program should generate the segmentation accordingly.</li>

 <li>You report must include a study of how changes in the various parameters affects the segmentation. Some parameters you could experiment with:

  <ul>

   <li>The number of iterations of GMM updating and energy minimization.</li>

   <li>The number of mixture components in your GMM.</li>

   <li>Whether to use soft GMM labels and do EM, and how that effects other parameters/results.</li>

   <li>Different ways to represent probabilities other than GMMs. 4-neighborhood or 8-neighborhood in your pairwise term.</li>

   <li>The choice of gamma.</li>

   <li>Alternative ways of setting beta.</li>

   <li>A tight initial bounding box or a loose bounding box.</li>

   <li>Better ways of using the bounding box for segmentation.</li>

   <li>Different color spaces or ways of representing pixels. Co-segmentation.</li>

  </ul></li>

</ol>

<h1>Stereo correspondence using MRFs Bonus</h1>

<ol>

 <li>Use the Markov Random Fields framework to generate the stereo matching for the pairs of images given in Assignment 2.</li>

</ol>

<ol start="2">

 <li>The report must include a comparison between this method and the methods you used in Assignment 2, with a qualitative explanation for your observation.</li>

 <li>Please include the code used in a new sub-directory mrf/ in the code/ directory. The report for this may be included in the previous question’s report.</li>

 <li>Bonus marks will be given based on the code and quality of results.</li>

</ol>