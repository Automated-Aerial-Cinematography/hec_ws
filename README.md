# hec_ws

1). Clone the hec_ws using git clone. 
2). Open the terminal at the location at which workspace was cloned and Enter the following commands.
	cd hec_ws
	source  devel/setup.bash
            roslaunch  hector_quadrotor_demo test_simple_world.launch
3) Open another terminal and clone the Motion-Planner repository and enter the following commands.
First source the hec_ws in this terminal 
	cd hec_ws
            source devel/setup.bash
           rosservice  call /enable_motors “enable: true”
            cd ..
            cd Motion-Planner
            python integration.py 
After this an image named ‘integration.png’ would be created in the folder which will show us the path that the quadrotor is going to follow.
            
