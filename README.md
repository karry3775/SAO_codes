# SAO_codes
A repository containing codes utilised for implementing a novel analytical method utilizing structures present in a warehouse environment. This is a supplemental repository for the paper titled "Structure Aided Odometry (SAO) : A novel analytical odometry technique based on semi-absolute localization for precision warehouse robotic assistance in environments with low feature variation."

# Content definition (in the order of appearance)

Content | Definition 
--- | --- 
urdf | This folder contains the urdf file of the pioneer2dx robot used for our experiments.
mesh | mesh files used for the robot model
block_counting.py | An independent code module used for getting the block count as explained in the paper.
coarse2fine.py | An independent code module used for converting the coarse block count states into fine estimates.

## NOTE:  block_counting and coarse2fine were used to implement SAO for isolated aisles experiments.

Content | Definition
-- | --
get_abs_ori.py | An independent code module used to get absolute orientation estimates from ceiling corrugation patterns
is_corridor_module.py | An independet code module implementing a basic aisle detection based on laser scan data.
laser_odom_corrected.py | An independent code module taking the absolute orientation estimates and using information from rf2o odometry to get odometry with yaw correction.
switch_and_esttimate.py | An independent code module which does the combined job of block_counting.py and coarse2fine.py along with implementation of a swtiching logic. This was the primary code for implementation of LPII as mentioned in the paper.

