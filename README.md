## Visual Odometry for Localization in Autonomous Driving

**A comparison of transformation reconstruction methods for optimal path estimates
using Feature Detection, Description, Matching and Trajectory Generation**


This project estimates an autonomous vehicle trajectory using a sequence of images taken with a monocular camera mounted on a vehicle. The images are from a CARLA autonomous driving simulator that include both RGB and grayscale versions. Depth maps for each image are also utilized.

Reconstruction of the transform between consecutive images consisting of a rotation matrix and translation vector necessary for the trajectory point calculations is made using three different methods: EMD (Essential Matrix Decomposition), PnP, (Perspective-n-Point), and PnP-RANSAC. 

A comparison of the trajectory results using EMD, PnP, and PnP-RANSAC
with both distance filtered and unflitered feature matches between images is done with visual plots of the trajectories.

The Jupyter notebook covers these areas:

- Explore the image set, depth maps, and intrinsic camera parameters
- Compare RGB and grayscale images
- Preprocess images with gaussian filtering
- Extract  features from the sequence of images
- Match features between consecutive images
- Create distance filtered and unfiltered matched pair sets for calculations
- Use matched feature pairs to estimate camera motion in 3D camera coordinate frame between images
- Build the trajectory paths using three transformation types: EMD, PnP, and PnP-RANSAC
- Plot out results for EMD, PnP, and PnP-RANSAC for both filtered and unflitered feature matching
- Compare results to find the best method
- Observations


This project is partially derived from a project in the University Of Tornoto course "Visual Perception for Self-Driving Cars"
