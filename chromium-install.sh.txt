#!/bin/bash

# ========== Banner ========== #
echo -e "\033[1;35m"
echo "====================================="
echo "       VenomRxz Auto Installer       "
echo "====================================="
echo -e "\033[0m"
sleep 1

# ========== Update & Install Chromium ========== #
echo "[+] Updating system..."
sudo apt update && sudo apt upgrade -y

echo "[+] Installing Chromium & dependencies..."
sudo apt install -y chromium-browser chromium-driver python3-pip
pip3 install selenium

echo -e "\n✅ \033[1;32mInstallation Complete - Powered by VenomRxz\033[0m"
