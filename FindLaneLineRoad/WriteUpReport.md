FindLaneLineRoad Project WriteUp
About the pipline
1. follow the step in the class to make the pipline
	a.grayscale the image by cv2.cvtColor
	b.blur the grayscale image use filter size as 3
	c.get the edges from the blurimage, use canny function of opencv
	d.make a ladder shape, mask the edges image
	e.get these lines from the mask image, use the houghLine function of opencv
	f.and draw these lines into a line image
	e.combine the orgin image and the line image
	g.save the combined image as the result

2. for the purpose of reduce the horizontal line, i dropout the lines which the points vertical distance is less than 100

The shortcomings:
1. actually , I am not very familiar with the houghLine function, the parmters, I just try some values. So these is not the best ones
2. some point which is white or yellow, in the mask, but are not in the lane lines, these will make some noise. I don't know how to reduce this situation

The Suggestions for improving
1. optimize the parmters
2. some new method to reduce the noise object
