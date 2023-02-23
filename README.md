# TagGraph
# The installation guide of TagGraph in WSL Ubuntu 22.04.5 LTS

#install pip
curl https://bootstrap.pypa.io/pip/2.7/get-pip.py --output get-pip.py # Fetch get-pip.py for python 2.7 
python2 get-pip.py
pip --version

#install MySQL-python
sudo apt-get install python2.7-dev default-libmysqlclient-dev build-essential
sudo wget https://raw.githubusercontent.com/paulfitz/mysql-connector-c/master/include/my_config.h -O /usr/include/mysql/my_config.h
sudo pip install MySQL-python

#Install non-standard packages with pip commands which TagGraph will need
pip install lxml==4.2.1
pip install numpy==1.7.1
pip install pyteomics==3.5.1
pip install sqlalchemy
pip install pandas==0.22.0
pip install pympler==0.5
pip install networkx==1.11
pip install pymzml==0.7.8
pip install matplotlib

#After installing these required packages, Navigate to the new folder that was created
D. Verify all required modules have been installed:
Run python checkPythonPackages.py




