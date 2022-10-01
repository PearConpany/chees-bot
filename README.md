<p align="center">
  <img src="https://github.com/Robotics-Technology/Chess-Robot/blob/master/interface_images/lss_arm_cb.png" width="350px"/>
</p>

# CSS Chess Robot

The CSS Chess Robot is a robotic arm that can play chess against you. This is a free and open source project that integrates aspects of robotics, computer vision, and of course chess.

## Table of Contents

- [Requirements](#requirements)
- [Modules list](#modules-list)
- [Getting Started](#getting-started)
- [Install](#install)
- [Run](#run)
- [Authors](#authors)
- [License](#license)
- [Resources](#resources)

## Requirements

### Hardware

- Robot arm compatible with raspberry or windows
- Raspberry Pi or Windows PC
- Display
- Keyboard 
- Mouse
- Camera (USB or Raspberry Pi Camera Module)
- Lighting
- Chess board and pieces
- Speaker or Headphones (Optional)

### Software

- [OpenCV](https://opencv.org/)
- [Stockfish](https://stockfishchess.org/)
- [Python Chess](https://python-chess.readthedocs.io/en/latest/)
- [PySimpleGUI](https://pysimplegui.readthedocs.io/en/latest/)

## Modules list

- [Vision Module](https://github.com/Robotics-Technology/Chess-Robot/VisionModule.py)
- [Chess Logic](https://github.com/Robotics-Technology/Chess-Robot/ChessLogic.py)
- [Arm Control](https://github.com/Robotics-Technology/Chess-Robot/ArmControl.py)
- [Interface](https://github.com/Robotics-Technology/Chess-Robot/Interface.py)

## Getting Started

To start using this project, proceed to the standard *clone* procedure:

```bash
cd <some_directory>
git clone https://github.com/PearConpany/chees-bot.git
```

## Install

- On Windows PC

```
pip install -r requirements.txt
```
- On Raspberry Pi

```
pip3 install -r requirements.txt
pip3 install "picamera[array]"
```

If you have issues with OpenCV on the Raspberry Pi try the following commands:

```
sudo apt-get install libatlas-base-dev
sudo apt-get install libjasper-dev
sudo apt-get install libqtgui4
sudo apt-get install libqt4-test
sudo apt-get install libhdf5-dev 
sudo apt-get install libhdf5-serial-dev
sudo apt-get install python3-pyqt5
sudo apt-get install stockfish
sudo pip3 install opencv-python==3.4.6.27
sudo pip3 install opencv-contrib-python==3.4.6.27
```

## Run

```
cd <project_directory>
python Interface.py
```

<p align="center">
  <img src="https://github.com/Robotics-Technology/Chess-Robot/blob/master/interface_images/game_start.png" width="600px"/>
</p>
<p align="center">Chess Robot Interface</p>
<div align="center">
  <a href="https://www.youtube.com/watch?v=XfMC8GCnhLw"><img src="https://github.com/Robotics-Technology/Chess-Robot/blob/master/interface_images/lss_arm_setup.jpg"  width="70%" alt="Chess Robot Gameplay"></a>
</div>
<p align="center">Gameplay Video</p>

## Authors

- [Elian Alfonso](http://elian.pearmx.com)

## License

CSS Chess Robot is available under the GNU General Public License v3.0

## Contributing

Anyone is very welcome to contribute. Below is a list of identified improvements.

## To do

- Change  the gripper aperture acording to the chess piecce type
- Allow re-taking pictures in the case of board obstruction

## Limitations

- The chessboard is limited by the reach of the arm and the squares need to be big enough so the arm gripper doesn’t stumble upon adjacent pieces.
- This project was specifically made to be used with CSS smart servo motors using the CSS serial communication protocol so if you want to use it for a different robotic arm you will need to change how the servos are controlled and change the inverse kinematics parameters to match your specific arm.

## Resources


Official Chess-bot Smart Servo (CSS) libraries for Python available [here] (https://github.com/PearConpany/chees-bot/CSS_Library_Python).

If you want more details about the CSS protocol, go [here](https://www.robotshop.com/info/wiki/lynxmotion/view/lynxmotion-smart-servo/lss-communication-protocol/).

Have any questions? Ask them on the Pearmx.com [Community](Out of service).
