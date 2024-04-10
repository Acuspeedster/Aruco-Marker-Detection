The public_test_cases folder contains 2 images of the markers which in total contains 5 ArUco markers.

An image might contain more than one ArUco marker placed at different positions and orientations.
For each ArUco marker, the following parameters should be determined -
Parameter	Description & Return Type
Marker ID	This is unique for each marker. Should be returned as an int value
Center coordinates	Both X and Y coordinates of the marker center combined should be printed as a list.
Each co-ordinate should be of int type
Orientation	This is defined as the angle at which the marker is placed w.r.t to the vertical.
Should be of int type
Corner Points	For each marker, the corner points should be added to a separate dictionary for plotting the figure

Figure 1: Sample Aruco Image with details marked

The Red Dot at the center represents the Center

The four other dots(Green, Gray, Yellow, and Pink) represent the Corner points

The number written in Red font is the the marker ID which is unique for a particular marker

The number written in Green font is the angle in which the marker is oriented w.r.t. to the vertical axis. From the vertical, the angles will be measured as shown in Figure 2


Figure 2: Angle measurement

The final output for each image should be printed as a Dictionary with each key, value pair as defined below

Key => ID of an ArUco marker

Value =>Details (center coordinates and angle) of that marker as a list

An example output for an image having 2 ArUcos is given below for reference:

ArUco_details_dict = {9: [[311, 490], 0], 3: [[158, 175], -22]}

The corner values should be added to a separate dictionary with

Key => ID of an ArUco marker

Value =>Details (center coordinates and angle) of that marker as an array

An example output for an image having 2 ArUcos is given below for reference:

ArUco_corners = {9: array([[211., 389.],[412., 389.],[412., 592.],[211., 592.]], dtype=float32), 3: array([[109., 46.],[284., 118.],[207., 304.],[ 33., 232.]], dtype=float32)}
