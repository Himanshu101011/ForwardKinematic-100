# ForwardKinematic-100

# Code Explanation
Function Inputs:

DH_params: A matrix where each row represents a link’s D-H parameters.
joint_types: A cell array indicating whether each joint is revolute ('R') or prismatic ('P').

Forward Kinematics Calculation:
The transformation matrix is initialized as an identity matrix.
A loop iterates over all joints to compute individual transformation matrices using the D-H parameters.
The transformations are accumulated to obtain the end-effector position.

Visualization:
Uses plot3 to visualize each link.
Uses scatter3 to mark joint positions in red.
The manipulator is displayed in a 3D coordinate system.

Final Output:
The final transformation matrix (position & orientation of the end-effector) is displayed.
