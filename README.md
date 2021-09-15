# Flask Web Application

This is the simple web application using Python Flask use for education purposes.
There are the steps required to get it working on linux.
* Install and update OS dependencies
* Install applicaton dependences
* Deploy the application source code
* Start the WEB Server

## 1. Install OS dependencies

Update and upgrade repo (Debian/Ubuntu)
```
sudo apt-get update && apt-get upgrade -y
```
Python and its dependencies
```
sudo apt-get install -y python3 python3-pip
```

## 2. Install app dependencies
Install Flask framework
```
pip3  install  flask
```

## 3. Deploy the app source code
Copy source to /opt dir
```
cp app.py /opt
```

## 4. Start the webserver
Start web command
```
FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port=5000
```

## 5. Test
Open a browser and try URL
```
http://<IP>:5000                            => Hello!
http://<IP>:5000/hello%20there              => Hello, my friend.
```
