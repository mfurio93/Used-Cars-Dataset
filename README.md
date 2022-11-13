# Used-Cars-Dataset

Manuel Furio - CC: 1118876500 - Career: Civil Engineering

Norbey Garcia - CC: 1038417080 - Career: Civil Engineering

Nicolas Perez - CC: 1037666280 - Career: Civil Engineering

Source (Kaggle): https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data

Source (World Bank): https://data.worldbank.org/indicator/SL.TLF.CACT.FE.ZS
Source (World Bank): https://data.worldbank.org/indicator/SL.TLF.ACTI.MA.ZS
Source (World Bank): https://data.worldbank.org/indicator/NY.GDP.MKTP.CD

CSVs have already been uploaded to a Google Drive folder from which the notebook automatically pulls it. Code below:

--------------------------------------------------------------------------------

from pydrive.auth import GoogleAuth
from google.colab import drive
from pydrive.drive import GoogleDrive
from google.colab import auth
from oauth2client.client import GoogleCredentials

auth.authenticate_user()
gauth = GoogleAuth()
gauth.credentials = GoogleCredentials.get_application_default()
drive = GoogleDrive(gauth)

file_id = 'FILE ID FROM THE SHAREABLE LINK'
download = drive.CreateFile({'id':file_id})
download.GetContentFile('NAME TO SAVE IT AS.extension')

--------------------------------------------------------------------------------

Youtube (2nd Document): https://www.youtube.com/watch?v=AlpJvyU8Njw

YouTube (Final Document): 
