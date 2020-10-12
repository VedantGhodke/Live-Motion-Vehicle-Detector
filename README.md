Recommended Steps:

  1) Read the video
  2) Preprocessing
  3) Capturing movement in video:

a) Two consecutive frames are required to capture the movement. If there is
movement in vehicle, there will be small change in pixel value in the current
frame compared to the previous frame. The change implies movement. So
capture the first 2 frames now.
  4) Adding gaussion blur for smoothening
  5) Find the movement in video
a) If vehicle is moving, there will be slight change in pixel value in the next frame
compared to previous frame. We then threshold the image. This will be useful further
for preprocessing. Pixel value below 30 will be set as 0(black) and above as
255(white)
  6) Extracting contours
