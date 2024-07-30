# Safari-Learning_Web
Safari e-learning is an application aimed to Leveraging technology and Education to create awareness about the effects of poaching. Somepeople pratice poaching due to lack of education, Ignorance, Poverty and Lack of food. Safari Learning will be able to improve both stability and upskill their knwoledge about the effects of poaching and the our main solutions to it. 

## Install Python

Django is a Python web framework, thus requiring Python to be installed on your machine. At the time of writing, Python 3.12 is the latest version.

## Checkout Safari E-Learning
   - [Safari E-Learning]()

### Installation Steps:

1. **Download Python**: 
   - Go to [Python Downloads Page](https://www.python.org/downloads/).
   - Click on the download button for the latest Python version.
   - Download the executable installer.

2. **Run the Installer**:
   - Run the downloaded installer.
   - Check the box next to "Install launcher for all users (recommended)".
   - Click "Install Now" to begin the installation process.

3. **Verify Installation**:
   - After installation, open the command prompt.
   - Check that the Python version matches the version you installed by executing:
     ```
     py --version
     ```

   The command should display the installed Python version. If it does, Python has been successfully installed on your machine.

## About pip

pip is a package manager for Python and is included by default with the Python installer. It helps to install and uninstall Python packages (such as Django!). For the rest of the installation, we’ll use pip to install Python packages from the command line.

## Setting up a virtual environment

It is best practice to provide a dedicated environment for each Django project you create. There are many options to manage environments and packages within the Python ecosystem, some of which are recommended in the Python documentation. Python itself comes with venv for managing environments which we will use for this guide.

To create a virtual environment for your project, open a new command prompt, navigate to the folder where you want to create your project and then enter the following:

```
py -m venv Pkyla
```
This will create a folder called ‘healthpass’ if it does not already exist and set up the virtual environment.
To activate the environment, run:
```
Pkyla\Scripts\activate.bat
```
The virtual environment will be activated and you’ll see “(Pkyla)” next to the command prompt to designate that.
Each time you start a new command prompt, you’ll need to activate the environment again.
using this
```
Pkyla\Scripts\activate.bat
```

## Install Django

Django can be installed easily using pip within your virtual environment.

In the command prompt, ensure your virtual environment is active, and execute the following command:

```
py -m pip install Django
```
After the installation has completed, you can verify your Django installation by executing the following command in the command prompt:

```
django-admin --version
```
## change directory to Wildlife_Learning
```
cd Wildlife_Learning
```
## clone git hub repo
```
git clonehttps://github.com/Kylapurity/Safari-Learning_Web.git

```
## install the dependencies
pip install -r requirements.txt

## check if errors are present in the app
```
python manage.py check
```
## run the django server
```
python manage.py runserver
```
## now copy this url to your browser
1. [Signup](http://127.0.0.1:8000/safari_learning/safari_user_signup/)
2. [LogIn](http://127.0.0.1:8000/safari_learning/safari_user_login/)
3. [LandingPage](http://127.0.0.1:8000/safari_learning/landing_page/)
4. [Homepage/Courses](http://127.0.0.1:8000/safari_learning/safari_user_homepage/)
5. [Interest](http://127.0.0.1:8000/safari_learning/interests/3/)
6. [Events](http://127.0.0.1:8000/safari_learning/book_event/)
7. [FAQ](http://127.0.0.1:8000/safari_learning/faq_page/)

 
There you would see a page showing the path you could add
after the link these paths are the first argument of the
path function e.g user_signup



# Working with the html file, css file and js file
navigate to this directory
```
cd \Kyla\Wildlife-Learning\Wildlife_Conservation_Education_Initiative>
```
list directories and you would see files and folders
```
ls
```
then would see static folder, then change directory to it
```
cd static
```
then inside of static list directories
```
ls
```
then you would see styles, scripts, and images folder
put css file in styles folder
```
cd styles
```
put javascript files in scripts folder
```
cd scripts
```
put images files in images folder
```
cd images
```
then move to the folder of the html files you are working on
```
cd Kyla\Wildlife-Learning\Wildlife_Conservation_Education_Initiative\safari_learning\templates>
```
In your file put this in the head tag of your html as the first thing before title, meta tags
```
{% load static %}
```
before calling the style sheet in the link tag, the js in the script tag, and images in the image tag
```
<link rel="stylesheet" href="{% static './styles/yourcssscript.css' %}">
```
```
<script src="{% static './scripts/yourjsscript.js' %}"></script>
```
```
<img src="{% static './images/yourimagefile.[jpeg,jpg,png]' %}">
```
**then go back to this on cmd not powershell, use cmd on vscode to be running this commands below**
```
cd Kyla\Wildlife-Learning\Wildlife_Conservation_Education_Initiative
```
the run this commands
```
python manage.py check
```
```
python manage.py runserver
```
then go back to the top of the readme to see what i said you should do after running this commands
**Use vscode powershell to actually edit the scripts i.e css, js, and html**