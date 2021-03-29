# Face-Recognition
A facial recognition system is a technology capable of matching a human face from a digital image against a database of faces. Here in these, project we have created a system in which it captures the User image using your webcam and make a dataset for that user using a particular naming format, and it will store the name in the database. Here, we are using MYSQL database to store the user name with an ID, than we will train the user image dataset to make a recognizer called Training Data(YML) File. In which than the recognizer file is used to detect the user. If present in the Database and if the system recognises it than it will show the name or it will show Unknown.

# Packages Used
<strong> MYSQL Connector </strong>
<strong> numpy </strong></br>
<strong> Opencv </strong></br>
<strong> Opencv-Contrib-Python </strong>
<strong> OS </strong>
<strong> Pillow </strong>

# Commands
Firstly, make sure you have all the packages if not install them by using the following commands in the working directory:<br>
:: pip install mysql-connector-python</br>
:: pip install numpy</br>
:: pip install opencv-python</br>
:: pip install opencv-contrib-python</br>
:: pip install os-win</br>
:: pip install Pillow</br>

# Command to Run the Program
:: Firstly, make a Database in the MYSQL(PHPMYADMIN), than run the <strong> create_database.py </strong> file, it will create a table in the database.<br>
:: After making the table, run the <strong> main.py </strong> file, it will use OpenSource Frontal Face XML file, to detect the user face and it will capture the images of the user present in front of the webcam. Those, images will be store in the Dataset folder and the username will be asked and it will be stored in the database.<br>
:: After, storing the name in the database, and creating the dataset, run the <strong> trainer.py </strong> file, it will use the dataset which was created in the previous step, and it will make a trainingData model(Recognizer Model) using LBPH Face Recognizer Algorithm.<br>
:: After, making the recognizer model, run the <strong> detector.py </strong> file, here it will open a video capture window and it will try to detect the user in front of the webcam, if the data is present in the dataset and model, than it will recognize the face or it will show unknown face.<br>

# Queries
If you have any Doubt OR Problem while running the program, do label an issue