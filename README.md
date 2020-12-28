# design and simulate 3 link / 3DOF Robot Arm using Python
# Simulation Output Animation : https://imgflip.com/gif/4rvknr

# Methodology
The robot inverse kinematics task is concerned with the recognition of the whole feasible and proper sets of joint variables that would understand the solution to find out the positions and orientations of the end effector. In the inverse kinematics problem would not specify constantly a unique solution compared with forward solution i.e., 
Number of solutions to be obtained for one end effector position to reach the specified position and orientation. Case I. Two Link Planar Manipulator Manipulator Consider a two link planer manipulator having link lengths l1, l2 and joint angles 1 and 2 to reach a desired position (Px, Py) as shown in Fig. 1. For this, inverse solution is derived from geometric approach as per the diagram shown in Fig. 2 is as follows:
px  l1 cos1   l2 cos1   2  (1)



Fig. 2: Geometric model for a 2 link manipulator
This arm contain two links, link 1 and link 2, the length of tese both links are  l1 and l2 respectively. It is consider that link 1 is fixed to the horizontal and making an angle θ1 with horizontal. One end of link 2 is connected to link 1 and make with horizontal θ2.
It is consider that the start point coordinate of link 1 is (X0, Y0) and end point coordinate of link 1 is (X1, Y1). similarly for link 2 start and end point coordinates are (X1, Y1) and (X2, Y2), respectively.
Let X0 = 0 and Y0 = 0.
From figure and use of trigonometry formula we can say that
X1 = l1. Cos (θ1)      Y1=l1. Sin (θ1)  
 X2=X1+l2. Cos(θ2)   Y2=Y1+l2. Sin(θ2)
By using this equation we will solve the problem.
To solve this problem first we provide some input data. This input data contain Arm length (l1 and l2), angle (θ1 and θ2) and the position of absolute coordinate(X0, Y0). After giving this data we will calculate the value of the other coordinates by using above equation. To calculate the values of the coordinate for different angles we will use for loop. By using the for loop we get position of the links for different angles. By using plot command we will get graphical form of data. This graphical data is save by there figure name and then we combine those figure to get animation of the robotics arm.

# References
- Chaitanyaa, G. and S. Reddy, 2016. Genetic algorithm
- based optimization of a two Link planar robot
- manipulator. Int. J. Lean Think., 7: 1-3.
- Chen, Q., S. Zhu and X. Zhang, 2015. Improved inverse
- kinematics algorithm using screw theory for a sixDOF robot manipulator. Int. J. Adv. Robotic Syst.,12: 140-140. DOI: 10.5772/60834
