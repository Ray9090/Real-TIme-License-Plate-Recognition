# Real-TIme-License-Plate-Recognition
Raspberryi pi and Python based Real Time License Plare Recognition

All dependecny or package I needed:
sudo apt update
sudo apt full-upgrade
sudo apt-get install libhdf5-dev -y 
sudo apt-get install libhdf5-serial-dev –y 
sudo apt-get install libatlas-base-dev –y 
sudo apt-get install libjasper-dev -y
sudo apt-get install libqtgui4 –y
sudo apt-get install libqt4-test –y
pip3 install opencv-contrib-python==4.1.0.25
sudo apt-get install tesseract-ocr
pip3 install pytesseract
pip3 install pyttsx3
pip3 install imutils
sudo apt-get install ssmtp

Set up email into configure file:
sudo nano /etc/ssmtp/ssmtp.conf

added these lines

root=postman
mailhub=smpt.gmail.com:587
AuthUser=myemail@gmail.com
AuthPass=myemailpassword
FromLineOverride=YES
UseSTARTTLS=YES

Troubleshooting: 
1. Syntext error: typeerror sendmail() missing 1 required positional argument 'msg'
   server.sendmail("?????","?????",text)
2. Low resulation camera 
3. Raspberry pi showed low voltage warning due to connect too much devices   
4. SMTP Authentication Error when sending email using gmail and python: Allow Less secure app access in Gmail
5. Check multi-thread or stop auto start script
6. Tesseract support only Python '>=3.5'
    install python latest version and use pip3 
7. rapberry pi error not found ip 93.93.128.193 80
   The apt mirror no longer contain the python-imaging library for the version of raspbian that I was using
   Needed to update and upgrading Raspbian
   sudo apt update
   sudo apt full-upgrade
