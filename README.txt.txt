*********************************************************************************************
Foodie Chatbot
*********************************************************************************************
-------------------------
Problem Statement:
-------------------------

An Indian startup named 'Foodie' wants to build a conversational bot (chatbot) which can help users discover restaurants across several Indian cities. You have been hired as the lead data scientist for creating this product.

The main purpose of the bot is to help users discover restaurants quickly and efficiently and to provide a good restaurant discovery experience.

-------------------------------------------------------
Achived below poimts with our Foodie Bot:
High level Summary:
-------------------------------------------------------
	** Bot Auto Greets the Customer
	** The bot takes city input from the customer as a text field.Foodie works only in Tier-1 and Tier-2 cities
	** The bot able to identify common synonyms of city names, such as Bangalore/Bengaluru, Mumbai/Bombay etc.
	**  Bot can able to identify tier-3 cities and it is replying back with something like "We do not operate in that area yet".
	** It takes the cuisine preference from the customer. The bot listing out the following six cuisine categories (Chinese, Mexican, Italian, American, South Indian & North Indian) and the customer can select any one out of that
	** Average budget for two people - Segment the price range (average budget for two people) into three price categories: lesser than 300, 300 to 700 and more than 700. The bot asking the user to select one of the three price categories
	** While showing the results to the user, the bot display the top 5 restaurants in a sorted order (descending) of the average Zomato user rating (on a scale of 1-5, 5 being the highest). The format be: {restaurant_name} in {restaurant_address} has been rated {rating}.
	** Finally, the bot ask the user whether he/she wants the details of the top 10 restaurants on email. If the user replies 'yes', the bot should ask for user’s email id and then send it over email. Else, just reply with a 'goodbye' message. The mail should have the following details for each restaurant:

		* Restaurant Name
		* Restaurant locality address
		* Average budget for two people
		* Zomato user rating

       	** We used Python Email Package
	** Complete Bot project is deployed in slack and tested with most complex conversational stories.

------------------
Prerequisites:
------------------
python 3.6.x, Visual studio for python development, Rasa X package

------------------------------
How to Install Rasa X?
------------------------------

** Rasa Instalation:

	# Create New Env
		conda create -n rasademo python=3.7

	# Checking created env
		conda info --envs

	# Activate rasa
		conda activate rasa

	# Checking Python Version
		python

	# Install RasaX
		pip install rasa-X --extra-index-url https://pypi.rasa.com/simple

	# Check Installed package and Version
		pip install rasa==1.9.5

	# Check Available version in rasa
		pip install rasa==

	# Install Spacy
	# Anaconda prompt Run as Administrator
		pip install rasa[spacy]==2.1.9
		python -m spacy download en_core_web_md
		python -m spacy link en_core_web_md en

-------------------------
Methods Used:
-------------------------

** NLU and Core Training:

	# Activate rasa
		activate rasademo

	# Train
		rasa train -vv -dump-stories --force

** Build actions for the bot. 

	* Read through the Zomato API documentation to extract the features such as the average price for two people and restaurant’s user rating. 
	* Also build an ‘action’ for sending emails from Python.

** Creating more stories - Post Installation, code development and NLU training - Run bot Interactive mode to capture stories:
	
	# Creating more stories - Interactive mode
		rasa interactive

** Test Foodie Bot in terminal:

	# Run actions
		rasa run actions

	# Open another prompt and run shell
		rasa shell

** Deployment : 
	# Created New Work Space and Deployed the model on Slack. 

** Deployment : Slack Testing
	# Post deployment multiple critical stories has been tested in slack


-------------------------
Softeware Required:
-------------------------
absl-py==0.9.0
aiofiles==0.5.0
aiohttp==3.6.2
alembic==1.4.2
APScheduler==3.6.3
astor==0.8.1
async-generator==1.10
async-timeout==3.0.1
attrs==19.3.0
blinker==1.4
blis==0.2.4
boto3==1.12.41
botocore==1.15.41
cachetools==4.1.0
certifi==2020.4.5.1
cffi==1.14.0
chardet==3.0.4
click==7.1.1
cloudpickle==1.2.2
colorama==0.4.3
colorclass==2.2.0
coloredlogs==10.0
colorhash==1.0.2
cryptography==2.9
cycler==0.10.0
cymem==2.0.3
decorator==4.4.2
dnspython==1.16.0
docopt==0.6.2
docutils==0.15.2
en-core-web-md==2.1.0
fbmessenger==6.0.0
Flask==1.1.2
Flask-Mail==0.9.1
future==0.18.2
gast==0.2.2
gevent==1.4.0
gitdb==4.0.4
GitPython==3.1.1
google-auth==1.14.0
google-auth-oauthlib==0.4.1
google-pasta==0.2.0
greenlet==0.4.15
grpcio==1.28.1
h11==0.8.1
h2==3.2.0
h5py==2.10.0
hpack==3.0.0
hstspreload==2020.4.14
httplib2==0.17.2
httptools==0.1.1
httpx==0.9.3
humanfriendly==8.1
hyperframe==5.2.0
idna==2.9
importlib-metadata==1.6.0
isodate==0.6.0
itsdangerous==1.1.0
Jinja2==2.11.2
jmespath==0.9.5
joblib==0.14.1
jsonpickle==1.3
jsonschema==3.2.0
kafka-python==1.4.7
Keras-Applications==1.0.8
Keras-Preprocessing==1.1.0
kiwisolver==1.2.0
Mako==1.1.2
Markdown==3.2.1
MarkupSafe==1.1.1
matplotlib==3.1.3
mattermostwrapper==2.2
multidict==4.7.5
murmurhash==1.0.2
networkx==2.4
numpy==1.18.2
oauth2client==4.1.3
oauthlib==3.1.0
opt-einsum==3.2.1
packaging==19.0
pandas==1.0.3
pika==1.1.0
plac==0.9.6
preshed==2.0.1
prompt-toolkit==2.0.10
protobuf==3.11.3
psycopg2-binary==2.8.5
pyasn1==0.4.8
pyasn1-modules==0.2.8
pycparser==2.20
pydot==1.4.1
PyJWT==1.7.1
pykwalify==1.7.0
pymongo==3.8.0
pyparsing==2.4.7
pyreadline==2.1
pyrsistent==0.16.0
PySocks==1.7.1
python-crfsuite==0.9.7
python-dateutil==2.8.1
python-editor==1.0.4
python-engineio==3.11.2
python-socketio==4.4.0
python-telegram-bot==11.1.0
pytz==2019.3
PyYAML==5.3.1
questionary==1.5.2
rasa==1.9.6
rasa-sdk==1.9.0
redis==3.4.1
requests==2.23.0
requests-oauthlib==1.3.0
requests-toolbelt==0.9.1
rfc3986==1.4.0
rocketchat-API==0.6.36
rsa==4.0
ruamel.yaml==0.15.100
s3transfer==0.3.3
sanic==19.12.2
Sanic-Cors==0.10.0.post3
sanic-jwt==1.3.2
Sanic-Plugins-Framework==0.9.2
scikit-learn==0.22.2.post1
scipy==1.4.1
six==1.14.0
sklearn-crfsuite==0.3.6
slackclient==2.5.0
smmap==3.0.2
sniffio==1.1.0
spacy==2.1.9
SQLAlchemy==1.3.16
srsly==1.0.2
tabulate==0.8.7
tensorboard==2.1.1
tensorflow==2.1.0
tensorflow-addons==0.9.1
tensorflow-estimator==2.1.0
tensorflow-hub==0.7.0
tensorflow-probability==0.7.0
termcolor==1.1.0
terminaltables==3.1.0
thinc==7.0.8
tqdm==4.31.1
twilio==6.26.3
typeguard==2.7.1
tzlocal==2.0.0
ujson==1.35
urllib3==1.25.9
wasabi==0.6.0
wcwidth==0.1.9
webexteamssdk==1.1.1
websockets==8.1
Werkzeug==1.0.1
wincertstore==0.2
wrapt==1.12.1
yarl==1.4.2
zipp==3.1.0

