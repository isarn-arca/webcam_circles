# webcam_circles

Circle detection from online webcam images

- **STEP 1: Fork the repository:**

https://github.com/beta-robots/webcam_circles

- **STEP 2: Clone the repository:**

`$ git clone https://github.com/beta-robots/webcam_circles.git`

- **STEP 3: Enter in the local folder webcam_point_features:**

`$ cd webcam_circles`

- **STEP 4: Create the directory "buil" in the local folder webcam_point_features:**

`$ mkdir build`

- **STEP 5: Enter in the directory "build":**

`$ cd build`

- **STEP 6: Compile:**

`$ cmake ..`

`$ make`

- **STEP 7: Execute:**

`$ ./circle_detector`

**Comment:**

You can see in this repository (folder "Images") the capture images of the webcam_circles

**Explanation about Hough Transform**

We can use the Hough Tranform to detect lines and circular shapes. The follow steps to do Hough Transform for circles are:
- create the accumulator space, which is made up of a cell for each pixel. Initially each cell is set to 0
- For each edge point (i, j) in the image, increment all cells which according to the equation of a circle (i-a)² + (j-b)² = r² could be the center of a circle
- For each possible value of a {\displaystyle a} a found in the previous step, find all possible values of b {\displaystyle b} b which satisfy the equation
- Search for local maxima in the accumulator space. These cells represent circles that were detected by the algorithm

## Tips

http://homepages.inf.ed.ac.uk/rbf/HIPR2/hough.htm

https://en.wikipedia.org/wiki/Hough_transform
