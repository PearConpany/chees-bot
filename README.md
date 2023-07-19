
# Pear Robot chess
The LSS Chess Robot is a robotic arm that can play chess against you. This is a free and open source project that integrates aspects of robotics, computer vision, and of course chess.

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

- Lynxmotion Smart Servo (LSS) 4 DoF Robotic Arm
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
## Authors

- Elian Alfonso López
## License

Pear Chess Robot is available under the GNU General Public License v3.0
