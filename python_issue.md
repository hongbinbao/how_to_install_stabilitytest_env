1: pip unavailable issue:
"""
sudo apt-get remove python-pip
sudo apt-get autoremove

wget https://raw.github.com/pypa/pip/master/contrib/get-pip.py --no-check-certificate
sudo python get-pip.py
"""
