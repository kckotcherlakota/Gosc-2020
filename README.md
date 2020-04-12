# GOOGLE SUMMER OF CODE -2020
### PROJECT DETAILS: PYTHON DEEP LEARNING INFERENCE ON VIDEO
### ORGANIZATION: OPENCV 

### ABSTRACT 
The goal of this project is to develop a high-level helper class in python to perform optimized inference on videos.for an improved video inference we use a new method of adaptive enhancement and upscaling of video feed ​. And impose a powerful topological prior to the bounding box , which prevents the solution from excessive shrinking and ensures that the user-provided box bounds the segmentation in a sufficiently tight way

### FEATURES 
1. Adaptive Enhancement functionality of the video feed
2. Upscaling functionality to the source video
3. Improved image segmentation with the bounding box using topological
prior

### Possible Mentors​: ​Justin Shenk

### PROJECT OBJECTIVES
1. To create individual add-on classes for adaptive enhancement and upscaling functionality which can easily be used.
2. To provide a custom value based customization for video enhancement and upscaling functionality
3. To create an add-on class for the image segmentation ​with the bounding box using topological prior

### MEASURABLE OUTCOMES:
1. To create individual add-on classes for adaptive enhancement and upscaling functionality which can easily be used.
2. To provide a custom value based customization for video enhancement and upscaling functionality
3. To create an add-on class for the image segmentation ​with the bounding box using topological prior
ACHIEVING PROJECT GOALS
The entire project can be broadly classified into three phases through completion
### Phase 1-​Deliverable before the first Mid-Term evaluation
1.1. Add-on class functionality for the video upscaling
1.2 creating database for the image segmentation 
1.3 testing various algorithms with our database 
1.4 building class for the image segmentation function ​with the bounding box using topological prior 
1.5 declaration of the validation parameters
### Phase 2-​Deliverable before the second Mid-Term evaluation
2.1 working on the custom value based customization for upscaling 
2.2 testing the video upscaling function 
2.3 building a add on class for the video enhancement functionality
2.4 testing image segmentation
### Phase 3-​Deliverable before the final evaluation
3.1 working on the custom value based customization for the video enhancement functionality 
3.2 testing all the three classed 
3.3 documentation of the parameters with minimum and maximum values for customization 
3.4 debugging of the classes along with the parameters
### Wishlist: ​
Can be implemented if all the above tasks are completed successfully and the programme is yet to end, also desired to be taken up post GSoC
● Additional class which uses the objects calls of all the above classes with a standardized value parameters, without individually calling the parameters for each sub classes

### DETAILED EXPLANATION :
For Video enhancement and upscaling ​we introduce a novel framework for adaptive enhancement and spatiotemporal upscaling of videos containing complex activities without explicit need for accurate motion estimation. Our approach is based on multidimensional kernel regression, where each pixel in the video sequence is approximated with a 3-D local series, capturing the essential local behavior of its spatiotemporal neighborhood. The coefficients of this series are estimated by solving a local weighted least-squares problem, where the weights are a function of the 3-D space-time orientation in the neighborhood. As this framework is fundamentally based upon the comparison of neighboring pixels in both space and time, it implicitly contains information about the local motion of the pixels across time, therefore rendering unnecessary an explicit computation of motions of modest size the proposed yields improved overall performance. And for the video upscaling we use , Fast and Accurate Image Upscaling With Super-Resolution Forest for each frame in the given video feed.

For the improved plot of bounding box we use image segmentation with the bounding box using topological prior, which prevents the solution from excessive shrinking and ensures that the user-provided box bounds the segmentation in a sufficiently tight way.the algorithm for building the prior is as follows, The prior is expressed using hard constraints incorporated into the global energy minimization framework leading to an NP-hard integer program. We then investigate the possible optimization strategies including linear relaxation as well as a new graph cut algorithm called pinpointing. The latter can be used either as a rounding method for the fractional LP solution, which is provably better than thresholding-based rounding, or as a fast standalone heuristic.A simple class can be built on top of this with all the processing done so that the user can use these features with a simple call of the library
