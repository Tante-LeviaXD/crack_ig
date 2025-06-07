#!/bin/bash

pkg update && pkg upgrade -y
pkg install python git -y

pip install requests colorama
pip install bs4
pip install lxml
pip install rich

git clone https://github.com/Tante-LeviaXD/crack_ig
cd crack_ig
python crack.py
