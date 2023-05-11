#!/bin/bash

# Download Google Chrome
wget -q https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

# Install Google Chrome silently
if [ -x "$(command -v dpkg)" ]; then
    # Ubuntu-based distribution
    sudo dpkg -i google-chrome-stable_current_amd64.deb > /dev/null 2>&1
elif [ -x "$(command -v yum)" ]; then
    # Red Hat or CentOS-based distribution
    sudo yum localinstall google-chrome-stable_current_amd64.deb -y > /dev/null 2>&1
else
    echo "Unsupported distribution."
fi

# Clean up downloaded file
rm google-chrome-stable_current_amd64.deb

echo "Google Chrome has been installed successfully."
