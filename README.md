# RL_CNN_Lateral_Control
Reinforcement Learning and CNN for Lateral Control for Autonomous Driving
Files:
1. Tf_steer_play
2. Torcs-1.3.7
3. Tracks


Dependencies:
1. Ubuntu 16.04
2.Python 2.7
3. Tensorflow 1.15.0
4. Opencv
5. sysv_ipc


TORCS Installation:
Open terminal in the Project Code folder.
1. sudo apt-get update
2. sudo apt-get install libglib2.0-dev libgl1-mesa-dev libglu1-mesa-dev freeglut3-dev libplib-dev libopenal-dev libalut-dev libxi-dev libxmu-dev libxrender-dev libxrandr-dev libpng12-dev libvorbis-dev xautomation
3. cd torcs-1.3.7
4. ./configure
5. make -j4
6. sudo make install 
7. sudo make datainstall


Creating Virtual Environment:
Create an isolated environment for the project. You can pip install required dependencies here. 
This is created in the tf_steer_play folder


1. sudo apt-get install virtualenv
2. virtualenv -p python2.7 torcs-env
3. source torcs-env/bin/activate
4. pip install tensorflow==1.15 sysv_ipc opencv-python


Simulation:
Open terminal in tf_steer_play folder. Activate the virtual environment.


Training: python main.py --mode train


Testing: python main.py --mode play


Configure Track:
To change the track from default. 
Terminal > torcs > race > practice > configure race > choose track > accept > run simulation as above
