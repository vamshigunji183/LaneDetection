# LaneDetection
## Libraries
  * OpenCV
  * matplotlib
  * numpy
  * moviepy
## Simple Step to achieve Lane Detection
  * converting image to grayscale image
    * `cv2.cvtColor`
  * apply GaussianBlur
    * `cv2.GaussianBlur`
  * Canny edge detection
    * `cv2.Canny`
  * ROI in opencv
    * blank masking
    * filling the pixels with the polygon defined by "vertices" with the fill color using ` cv2.fillPoly`
    * masking the image for `image only where mask pixels are nonzero` using `cv2.bitwise_and`
    * canny formed image is used as input to the `cv2.HoughLinesP`
      * drawing the line using slope (this is an interesting geomentric problem to solve)
    * `image` is the output of the `hough_lines()`, An image with lines drawn on it.Should be a blank image (all black) with lines drawn on it.
    
 <a href="https://youtu.be/kzGJZ7QF50k" target="_blank"><img src="https://youtu.be/kzGJZ7QF50k"alt="Demo" width="240" height="180" border="10" /></a>
      
