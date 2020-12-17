# How to open the app
- First, install Anaconda3. You can use conda_install.sh or you can go to https://docs.anaconda.com/anaconda/install/ for more details.
## If you are a Linux user
- Modify the configuration file (configuration.json).
- Run startApp.sh. You should specify the directory where the Anaconda is installed. For example,
$ ./startApp.sh /home/shared
## If you would like to run the program by yourself
- The app is running in conda virtual environment. To install all required packages, run
$ conda create --name \<env> --file requirements.txt
- Activate the virtual environment.
$ conda activate \<env>
- Go into the folder where the DicomAnnotator folder stored
$ cd /path/to/dir
- Then run
$ export PYTHONPATH="\$PYTHONPATH:$PWD"
- Modify the configuration file (configurations.json)
- Run the app by
$ python DicomAnnotator/main.py