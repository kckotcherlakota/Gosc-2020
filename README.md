# Gosc-2020

###                                      Google Summer Of Code ‘20 
### PROJECTPROPOSAL
### ORGANIZATION: ​OpenCV PYTHON DEEP LEARNING INFERENCE ON VIDEO
### NAME AND CONTACT INFORMATION
### NAME ​- N.V.M.K.CHAITANYA KOTHCERLAKOTA 
### EMAIL​-outreach.datadev@gmail.com 
### IRC/GITHUB​- kckotcherlakota
Phone number​ -+1 608-556-9176 Country/Region​- Madison,Wisconsin,USA
UNIVERSITY AND CURRENT ENROLLMENT
CURREN UNIVERSITY​- University Of Wisconsin-Madison
FIELD OF STUDY​- Computer Science Engineering
ABOUT ME
I am a third year undergraduate student studying Computer Science Engineering at University Of Wisconsin,Madison. I’m passionate about Machine learning and Artificial intelligence . I got introduced to machine learning in my freshman year and since then I’ve been trying out new frameworks and contributing a variety of projects. Most of my time goes developing applications based on machine learning ,discovering new research papers,and understanding them . I am an
  
 avid internet user and a regular reader of the tech forums like HackerNews, Reddit etc.
I successfully achieved many international hackathons like MS-hacks,LA-hacks and Eth Denver..etc, for developing various software applications. I also volunteered to give tech-talks in organizations like AI-saturdays ,PyData. I have a great exposure in the industrial aspect of application development, I was fortunate enough to work as an AI-intern in a startup “WhistleDrive”. I also worked as a Python teaching assistant for Minerva KGI Schools,SanFrancisco.My motivation to participate in the GSOC-2020 is to work on a challenging project under the guidance of a mentor which would enhance my skills and provide me with good experience.
PROJECT DETAILS
Abstract
The goal of this project is to develop a high-level helper class in python to perform optimized inference on videos.for an improved video inference we use a new method of adaptive enhancement and upscaling of video feed ​. And impose a powerful topological prior to the bounding box , which prevents the solution from excessive shrinking and ensures that the user-provided box bounds the segmentation in a sufficiently tight way
Features​:
1. Adaptive Enhancement functionality of the video feed
2. Upscaling functionality to the source video
3. Improved image segmentation with the bounding box using topological
prior
Possible Mentors​: ​Justin Shenk
MEASURABLE OUTCOMES:
1. To create individual add-on classes for adaptive enhancement and upscaling functionality which can easily be used.

 2. To provide a custom value based customization for video enhancement and upscaling functionality
3. To create an add-on class for the image segmentation ​with the bounding box using topological prior
ACHIEVING PROJECT GOALS
The entire project can be broadly classified into three phases through completion
Phase 1-​Deliverable before the first Mid-Term evaluation
1.1. Add-on class functionality for the video upscaling 1.2 creating database for the image segmentation 1.3 testing various algorithms with our database 1.3 building class for the image segmentation function ​with the bounding box using topological prior 1.4 declaration of the validation parameters
Phase 2-​Deliverable before the second Mid-Term evaluation
2.1 working on the custom value based customization for upscaling 2.2 testing the video upscaling function 2.3 building a add on class for the video enhancement functionality 2.4 testing image segmentation
Phase 3-​Deliverable before the final evaluation
3.1 working on the custom value based customization for the video enhancement functionality 3.2 testing all the three classed 3.3 documentation of the parameters with minimum and maximum values for customization 3.4 debugging of the classes along with the parameters
Wishlist: ​Can be implemented if all the above tasks are completed successfully and the programme is yet to end, also desired to be taken up post GSoC
● Additional class which uses the objects calls of all the above classes with a standardized value parameters, without individually calling the parameters for each sub classes

 DETAILED EXPLANATION :
For Video enhancement and upscaling ​we introduce a novel framework for adaptive enhancement and spatiotemporal upscaling of videos containing complex activities without explicit need for accurate motion estimation. Our approach is based on multidimensional kernel regression, where each pixel in the video sequence is approximated with a 3-D local series, capturing the essential local behavior of its spatiotemporal neighborhood. The coefficients of this series are estimated by solving a local weighted least-squares problem, where the weights are a function of the 3-D space-time orientation in the neighborhood. As this framework is fundamentally based upon the comparison of neighboring pixels in both space and time, it implicitly contains information about the local motion of the pixels across time, therefore rendering unnecessary an explicit computation of motions of modest size the proposed yields improved overall performance. And for the video upscaling we use , Fast and Accurate Image Upscaling With Super-Resolution Forest for each frame in the given video feed.
For the improved plot of bounding box we use image segmentation with the bounding box using topological prior, which prevents the solution from excessive shrinking and ensures that the user-provided box bounds the segmentation in a sufficiently tight way.the algorithm for building the prior is as follows, The prior is expressed using hard constraints incorporated into the global energy minimization framework leading to an NP-hard integer program. We then investigate the possible optimization strategies including linear relaxation as well as a new graph cut algorithm called pinpointing. The latter can be used either as a rounding method for the fractional LP solution, which is provably better than thresholding-based rounding, or as a fast standalone heuristic.A simple class can be built on top of this with all the processing done so that the user can use these features with a simple call of the library

 References:
1. X. Li and Y. Zheng, "Patch-Based Video Processing: A Variational Bayesian Approach," in ​IEEE Transactions on Circuits and Systems for Video Technology​, vol. 19, no. 1, pp. 27-40, Jan. 2009
2. H. Takeda, P. Milanfar, M. Protter and M. Elad, "Super-Resolution Without Explicit Subpixel Motion Estimation," in IEEE Transactions on Image Processing, vol. 18, no. 9, pp. 1958-1975, Sept. 2009.

 3. L. Jin, S. Satoh and M. Sakauchi, "A novel adaptive image enhancement algorithm for face detection," Proceedings of the 17th International Conference on Pattern Recognition, 2004. ICPR 2004., Cambridge, 2004, pp. 843-848 Vol.4.
4. https://github.com/opencv/opencv/wiki/GSoC_2020#opencv-project-ideas-list
5. http://vision.stanford.edu/teaching/cs231b_spring1213/papers/lkrs_iccv09_TR.pdf
6. https://dl.acm.org/doi/10.1109/TIP.2009.2023703#d2464872e1
   
 
