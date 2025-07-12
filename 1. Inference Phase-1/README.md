# GUI Application Installation steps:

## Windows:
**1. Python:**

Download Python from [link](https://www.python.org/downloads/).

Version 3.8 or above is preferred.

Run the below command in cmd and check the version:
```
python --version
```
**2. Node.js:**

Download Node js from [link](https://nodejs.org/en/download).

Version 18 or above is preferred.

Run the below command in cmd and check the version.
```
node --version
```

After completing all the installations, clone the training model GUI to perform data annotations.

#### Download the code 
1. Open the below link and download the "gui_for_dlmodel" folder.
   
   [Link](https://iith-my.sharepoint.com/personal/ai23mtech02003_iith_ac_in/_layouts/15/onedrive.aspx?ga=1&id=%2Fpersonal%2Fai23mtech02003%5Fiith%5Fac%5Fin%2FDocuments%2FOffloading%2DUGVApps%2DTiE%2FCode)

#### Installations for YOLO and labelImg tool
1. Open visual studio code and open the downloaded folder (gui_for_dlmodel) in it.
2. Go to the image-uploader directory by running the below command
   ```
   cd image-uploader
   ```
   
Run the below command in cmd to install npm.
```
npm install
```
3. Go to the YOLOv5 directory by running the below command
   ```
   cd image-uploader\public\yolov5
   ```
4. Run the below command to install the dependencies of YOLOv5:
   ```
   python -m pip install -r requirements.txt
   ```
5. Go to public directory.
   ```
   cd ..
   ```
6. Go to labelImg directory.
   ```
   cd labelImg
   ```
7. Run the below command to install the dependencies of labelImg tool:
   ```
   python -m pip install -r requirements\requirements-linux-python3.txt
   ```
   Install PyQt5:
   ```
   pip install PyQt5   
   ```
   Install lxml:
   ```     
   pip install lxml
   ```
   Run labelImg: Once you're in the correct directory, run the labelImg.py script using Python:
   ```   
   python labelImg.py
   ```
   This should open up the labelImg graphical user interface, which is used for annotating images.
#### Run the GUI
Run the below command to run the GUI:
```
npm start 2>&1 | Tee-Object -FilePath "output.txt"
```
Then open http://localhost:8000 in browser.

## Ubuntu Linux:

       sudo apt-get install pyqt5-dev-tools
       sudo pip3 install -r requirements/requirements-linux-python3.txt
       make qt5py3
       python3 labelImg.py
          
   This should open up the labelImg graphical user interface, which is used for annotating images.
11. Installations for Yolo model:
    ```bash
    cd yolov5
    pip install -r requirements.txt  # install
    ```
#### Usage <a id="usage"></a>
**1. Python:**
Check for the python version in terminal.
```
python --version
```
**2. Node.js:**
Run the below commands in terminal to install node js.
```
sudo apt update
sudo apt install nodejs
node -v
```
**3. npm:**

Run the below command in cmd to install npm.
```
sudo apt update
sudo apt install npm -y
npm –version
```

After completing all the installations, clone the training model GUI to perform data annotations.

#### Download the code 
1. Open the below link and download the "gui_for_dlmodel" folder.
   
   [Link](https://iith-my.sharepoint.com/personal/ai23mtech02003_iith_ac_in/_layouts/15/onedrive.aspx?ga=1&id=%2Fpersonal%2Fai23mtech02003%5Fiith%5Fac%5Fin%2FDocuments%2FOffloading%2DUGVApps%2DTiE%2FCode)

#### Installations for YOLO and labelImg tool
1. Open visual studio code and open the downloaded folder (gui_for_dlmodel) in it.
2. Go to the YOLOv5 directory by running the below command
   ```
   cd image-uploader\public\yolov5
   ```
3. Run the below command to install the dependencies of YOLOv5:
   ```
   python -m pip install -r requirements.txt
   ```
4. Go to public directory.
   ```
   cd ..
   ```
5. Go to labelImg directory.
   ```
   cd labelImg
   ```
6. Run the below command to install the dependencies of labelImg tool:
   ```
   python -m pip install -r requirements\requirements-linux-python3.txt
   ```
   Install PyQt5:
   ```
   pip install PyQt5   
   ```
   Install lxml:
   ```     
   pip install lxml
   ```
   Run labelImg: Once you're in the correct directory, run the labelImg.py script using Python:
   ```   
   python labelImg.py
   ```
   This should open up the labelImg graphical user interface, which is used for annotating images.
#### Run the GUI
Run the below command to run the GUI:

Go to the path: gui_for_dlmodel\image-uploader>


**Windows command:**
Then run:
```
npm start 2>&1 | Tee-Object -FilePath "output.txt"
```
**Ubuntu command:**
```
npm start 2>&1 | tee output.txt
```
Then open http://localhost:8000 in browser.

#### GUI demo
To easily navigate through the application, watch the GUI demo video and follow along with the step-by-step instructions provided in it.
https://github.com/TiHAN-Hyderabad/UGV-Object-Detection-21-Class-Model-Training/tree/main/Inference%20Phase-1/GUI_Demo_Video
