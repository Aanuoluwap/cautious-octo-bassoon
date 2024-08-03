**QuadPlot: A MATLAB Class for Visualizing Quadrotor Motion**

**Overview**

QuadPlot is a MATLAB class designed to visualize the motion of a quadrotor in 3D space. The class provides a simple and intuitive way to plot the quadrotor's position, orientation, and motor positions over time.

**Features**

Visualize quadrotor motion in 3D space

Plot quadrotor position, orientation, and motor positions

Update plot in real-time as new data is received

Supports multiple quadrotors with different colors and labels

Includes a built-in quaternion to rotation matrix conversion function (QuatToRot)

**Usage**

To use the QuadPlot class, simply create an instance of the class and pass in the necessary parameters, such as the quadrotor's initial state, wingspan, height, and color. Then, call the UpdateQuadPlot method to update the plot with new data.

Here is an example:

% Create a new QuadPlot instance
q = QuadPlot(1, [0 0 0 0 0 0 1 0], 0.5, 0.1, 'red');

% Update the plot with new data
q.UpdateQuadPlot([0.1 0.2 0.3 0 0 0 1 0], 0.1);

**Methods**

The QuadPlot class has the following methods:

'QuadPlot': The constructor method, which initializes the quadrotor's state and plot handles.

'UpdateQuadState': Updates the quadrotor's state with new data.

'UpdateQuadHist': Updates the quadrotor's history with new data.

'UpdateMotorPos': Updates the motor positions based on the quadrotor's state.

'TruncateHist': Truncates the quadrotor's history to a specified length.

'UpdateQuadPlot': Updates the plot with new data.

**Dependencies**

The QuadPlot class depends on the following functions:

'quad_pos': A function that calculates the coordinates of the quadrotor's position in the world frame.

'QuatToRot': A function that converts a quaternion to a rotation matrix.

**License**

The QuadPlot class is released under the MIT License. See the LICENSE file for details.

**Author**

The QuadPlot class was written by Aanuoluwap.
