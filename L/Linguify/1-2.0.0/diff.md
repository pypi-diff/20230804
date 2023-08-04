# Comparing `tmp/Linguify-1.tar.gz` & `tmp/Linguify-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Linguify-1.tar", last modified: Sun Jul 30 06:25:31 2023, max compression
+gzip compressed data, was "Linguify-2.0.0.tar", last modified: Fri Aug  4 18:21:10 2023, max compression
```

## Comparing `Linguify-1.tar` & `Linguify-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:25:31.939453 Linguify-1/
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:25:31.938688 Linguify-1/Linguify.egg-info/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      205 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/PKG-INFO
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      244 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/SOURCES.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/dependency_links.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       44 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/entry_points.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       92 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/requires.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        9 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/top_level.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      205 2023-07-30 06:25:31.939365 Linguify-1/PKG-INFO
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:25:31.939235 Linguify-1/linguify/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)    19136 2023-07-29 09:18:45.000000 Linguify-1/linguify/Linguify.py
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 02:57:11.000000 Linguify-1/linguify/__init__.py
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-07-30 06:25:31.939488 Linguify-1/setup.cfg
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      562 2023-07-30 06:23:56.000000 Linguify-1/setup.py
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-04 18:21:10.213133 Linguify-2.0.0/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)     1073 2023-08-01 04:06:37.000000 Linguify-2.0.0/LICENSE
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-04 18:21:10.211553 Linguify-2.0.0/Linguify.egg-info/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      231 2023-08-04 18:21:10.000000 Linguify-2.0.0/Linguify.egg-info/PKG-INFO
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      269 2023-08-04 18:21:10.000000 Linguify-2.0.0/Linguify.egg-info/SOURCES.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-08-04 18:21:10.000000 Linguify-2.0.0/Linguify.egg-info/dependency_links.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       44 2023-08-04 18:21:10.000000 Linguify-2.0.0/Linguify.egg-info/entry_points.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       92 2023-08-04 18:21:10.000000 Linguify-2.0.0/Linguify.egg-info/requires.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        9 2023-08-04 18:21:10.000000 Linguify-2.0.0/Linguify.egg-info/top_level.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      231 2023-08-04 18:21:10.213036 Linguify-2.0.0/PKG-INFO
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-08-04 18:21:10.212599 Linguify-2.0.0/linguify/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       71 2023-08-02 05:33:49.000000 Linguify-2.0.0/linguify/__init__.py
+-rwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)    20789 2023-08-04 17:53:20.000000 Linguify-2.0.0/linguify/linguify.py
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)    20692 2023-08-04 17:53:36.000000 Linguify-2.0.0/linguify/main.py
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-08-04 18:21:10.213176 Linguify-2.0.0/setup.cfg
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      591 2023-08-04 18:02:18.000000 Linguify-2.0.0/setup.py
```

### Comparing `Linguify-1/linguify/Linguify.py` & `Linguify-2.0.0/linguify/linguify.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,48 @@
+from main import start
 import email
 import smtplib
 import imaplib
 import os
 import openai
 import docx
 import datetime
 from googleapiclient.discovery import build
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from google.auth.transport.requests import Request
 import base64
 import click
 import mimetypes
+import sys
+import json
+
 
 
 ''' Command-Line Interface (CLI) functions'''
 
 
 
 @click.command()  # This is click syntax
-@click.option('--pathway', default='credentials.json')
-def start(pathway):
+
+def start():
     business_name = True
     while business_name:
         company = click.prompt('Enter Company Name')
         if len(company)>3:
             business_name = False
         else:
             click.echo("Company name must be over 3 characters")
     mail = False
     click.echo('Select the Email of your choice!')
     while not mail:
         email_choice = click.prompt('Gmail or Outlook')
         if email_choice.lower() == 'gmail':
             mail = True
-            credentials_file = 'credentials.json'
+            credentials_file = get_credentials_path()
             if not is_user_authenticated(): # Check if the user is already authenticated
                 login(credentials_file)
             click.echo("You are logged in.")
             check_email_for_voicemails(credentials_file,company)
         elif email_choice.lower() == 'outlook':
             # Connect to the IMAP server and login
             mail = True
@@ -53,36 +57,36 @@
                     click.echo(e)
         else:
             click.echo('Invalid Email.')
 
     print(f"\nThank you for using Linguify!\n")
 
     
+def get_credentials_path():
+    # Get the path of the current script (main.py) or module using __file__
+    current_file_path = os.path.abspath(__file__)
+
+    # Create the path to the "credentials" folder (located in the same directory as main.py)
+    credentials_folder = os.path.join(os.path.dirname(current_file_path), "credentials")
+
+    # Combine with the filename to get the full path to credentials.json
+    credentials_path = os.path.join(credentials_folder, "credentials.json")
+    return credentials_path
+    
 
-def login(credentials_file):
+def login(file_path):
     """Authorize the application to access Gmail."""
     
     # Get the Gmail API service to initiate the OAuth2 flow
-    file_path = os.path.abspath(credentials_file)
     service = get_gmail_service(file_path)
 
     # Redirect the user to the Google sign-in page to grant permission
     flow = InstalledAppFlow.from_client_secrets_file(file_path, SCOPES)
     auth_url, _ = flow.authorization_url(prompt='consent', request_uri=None)
-    '''print(f"Please visit the following URL to authorize the application:\n{auth_url}\n\n")
-
-    # Prompt the user to enter the authorization code after granting permission
-    auth_code = input("Enter the authorization code from the URL above: ")
-
-    # Exchange the authorization code for access token and refresh token
-    flow.fetch_token(authorization_response=auth_code)
 
-    # Save the credentials for future use
-    with open('token.json', 'w') as token:
-        token.write(flow.credentials.to_json())'''
 
 def is_user_authenticated():
     try:
         creds = Credentials.from_authorized_user_file('token.json', SCOPES)
         return creds.valid
     except:
         return False
@@ -108,18 +112,18 @@
     except:
         raise Exception('Incorrect username or password!')
 
     # Search for voicemail emails
     print("You are logged in!")
     print("Searching through emails for New Voicemails...")
     status, response = mail.search(None, "UNSEEN", 'SUBJECT "Voicemail"')
+    voice_processed = False
     if status == "OK":
         email_ids = response[0].split()  
         if len(email_ids)>0:
-            voice_processed = False
             for email_id in email_ids:
                 # Retrieve the email with the voicemail attachment
                 status, email_data = mail.fetch(email_id, "(RFC822)")
                 if status == "OK":
                     raw_email = email_data[0][1]
                     email_message = email.message_from_bytes(raw_email)
                     for part in email_message.walk():
@@ -142,16 +146,14 @@
                         print(f'Voicemail {voicemailCount}/{len(processed_content)} has been successfully processed!')
                     else:
                         print(f'Voicemails {voicemailCount}/{len(processed_content)} have been successfully processed!')
                     voicemailCount+=1
                     voice_processed = True
                 except KeyError:
                     pass
-        if voicemailCount == 1:
-            print('There are no New Voicemails!')  # Incase there's an email with voicemail as subject but no voicemail attachments
                     
         if voice_processed:
             send_email_notification_OUTLOOK(company,voicemailCount-1)
             
         else:
             print('There are no New Voicemails!')
 
@@ -163,19 +165,19 @@
     # Compose the email notification
     subject = f"Linguify Usage Notification: {company}"
     message = f"Company Name: {company}\nDate: {date} \nTranscriptions: {transcriptions} voicemail(s)\nTotal Cost: {transcriptions} x $4.59 = ${transcriptions*4.59}"  # Do you want to add GST
 
     # Connect to the SMTP server and login
     server = smtplib.SMTP("smtp.office365.com", 587)
     server.starttls()
-    server.login("abdul_khafagy2004@hotmail.com", 'Edmonton2011')
+    server.login("linguify@hotmail.com", 'L1ngu1fy@))$')
 
     # Send the email notification
     email_body = f"Subject: {subject}\n\n{message}"
-    server.sendmail("abdul_khafagy2004@hotmail.com", "abdul_khafagy2004@hotmail.com", email_body)  # (From, To, Message)
+    server.sendmail("linguify@hotmail.com", "abdul_khafagy2004@hotmail.com", email_body)  # (From, To, Message)
 
     # Close the connection to the SMTP server
     server.quit()
 
 
 
 
@@ -186,33 +188,45 @@
             mime_type = part.get_content_type()
             if format in mime_type:
                 attachment_data = part.get_payload(decode=True)
                 if verify:
                     return attachment_data,mime_type,format
         return None,None,None
     else:
-                print("Converting Voicemail into audio file...")
-                ext = mimetypes.guess_extension(mime)
-                if ext is None:
-                    ext = f'.{formats}'
+        print("Converting Voicemail into audio file...")
+        ext = mimetypes.guess_extension(mime)
+        if ext is None:
+            ext = f'.{formats}'
+    
+        if sys.platform.startswith('win'):
+            desktop_path = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
+        elif sys.platform.startswith('darwin') or sys.platform.startswith('linux'):
+            desktop_path = os.path.join(os.path.expanduser("~"), "Desktop")
+        else:
+            raise Exception("Unknown operating system.")
+        new_folder_path = os.path.join(desktop_path, 'Linguify_Voicemails')
+        try:
+            # Create the new folder
+            os.mkdir(new_folder_path)
         
-                filename =os.path.abspath(f'voicemails')  
-                if not os.path.isdir(f'{filename}/{date}/'):
-                    filename = os.path.join(filename,f'{date}')
-                    os.mkdir(filename)
-                    filename = os.path.abspath(filename)+f'/{voicemailCount}{ext}'
-                else:
-                    filename = filename+f'/{date}/{voicemailCount}{ext}'
-                # Save the voicemail attachment as a file
-                with open(filename, "wb") as attachment_file:
-                    attachment_file.write(ready_attachment_data)
-
-                # Process the voicemail attachment
-                print('AI Processing audio file...')
-                process_audio_file(filename)
+        #print(f"Folder '{folder_name}' created on the desktop.")
+        except FileExistsError: 
+            pass
+        if not os.path.isdir(f'{new_folder_path}/{date}/'):
+            filename = os.path.join(new_folder_path,f'{date}')
+            os.mkdir(filename)
+            filename = os.path.abspath(filename)+f'/{voicemailCount}{ext}'
+        else:
+            filename = f'{new_folder_path}/{date}/{voicemailCount}{ext}'
+        with open(filename, "wb") as attachment_file:
+            attachment_file.write(ready_attachment_data)
+
+            # Process the voicemail attachment
+        print('AI Processing audio file...')
+        process_audio_file(filename)
                 
 
 
 
 """
 These libraries provide essential functionalities for different aspects of Linguify: Gmail Edition. os allows you to interact with the file system,
 imaplib facilitates communication with IMAP servers for email retrieval, smtplib enables sending email notifications through SMTP
@@ -232,15 +246,15 @@
 
 """Gmail preferences:"""
 
 def send_email_notification(credentials_file_path,company,transcriptions):
     # Compose the email notification
     
     message = email.message.EmailMessage()
-    message['From'] = 'abdul_khafagy2004@hotmail.com'
+    message['From'] = 'linguify@hotmail.com'
     message['To'] = 'abdul_khafagy2004@hotmail.com'
     message['Subject'] = f"Linguify Usage Notification: {company}"
     message.set_content(f"Company Name: {company}\nDate: {date} \nTranscriptions: {transcriptions} voicemail(s)\nTotal Cost: {transcriptions} x $4.59 = ${transcriptions*4.59}")  # Do you want to add GST
 
 
     '''# Get the Gmail API service'''
     service = get_gmail_service(credentials_file_path)
@@ -255,54 +269,87 @@
     try:
         service.users().messages().send(userId='me', body=email_message).execute()
     
     except Exception as e:
         print(f"Error: {e}\nPlease contact the provider (abdul_khafagy2004@hotmail.com).\n")
 
 
+def get_api_key():
+    
+    # Load the API key from the configuration file
+    config_file_path = os.path.join(os.path.dirname(__file__), 'config.json')
+    with open(config_file_path, 'r') as config_file:
+        config_data = json.load(config_file)
+        api_key = config_data.get("openai_api_key")
+
+    if api_key == 'YOUR_OPENAI_API_KEY_HERE':
+        api_key = input("Please enter your OpenAI API key: ")
+        data = {"openai_api_key": api_key}
+        with open(config_file_path, "w") as file:
+            json.dump(data, file)
+
+    # Initialize the OpenAI API with the retrieved key
+    return api_key
+
+
+
 
 def process_audio_file(file):
     global voicemailCount
-    openai.api_key = "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"  # How will I make this universal
+    openai.api_key = get_api_key()  
     openai.Model.list()
 
     # Processing the voicemail
     audio_file = open(file, "rb")
     transcript = openai.Audio.transcribe(
         model="whisper-1", 
         file=audio_file, 
         prompt='Format it in point form.'
         )
     transcript=transcript['text']
     
     # Drafting the formatted response
-    data=[ {"role": "system", "content": "Respond in this format and add what you may think are important and relevant comments in the additional comments section: Name of costumer: \nAppointment Booking: \nRequested Procedure: \nDate and Time of appointment: \nPossible complications: \nAny further inquiries: \nAdditional Comments:"}]
+    data=[ {"role": "system", "content": "Respond in this format and add what you may think are important and relevant comments for the clinic to know based on the voicemail in the additional comments section: Name of patient: \nAppointment Booking: \nRequested Procedure: \nDate and Time of appointment: \nPossible complications: \nAny further inquiries: \nAdditional Comments:"}]
     data.append({"role": "user", "content": transcript})
     completion = openai.ChatCompletion.create(
     model="gpt-3.5-turbo",
     messages=data
     )
     response = completion.choices[0].message['content']
     #data.append({"role": "assistant", "content": response})
 
     # Creating the Word document
-    print('Creating Word Document...')
-    file_path = os.path.abspath('wordoc')
-    file_pathway = file_path+f'/{date}.docx'
-    if not os.path.exists(file_pathway):
-        document = docx.Document()
+    if sys.platform.startswith('win'):
+        desktop_path = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
+    elif sys.platform.startswith('darwin') or sys.platform.startswith('linux'):
+        desktop_path = os.path.join(os.path.expanduser("~"), "Desktop")
     else:
+        raise Exception("Unknown operating system.")
+    new_folder_path = os.path.join(desktop_path, 'Linguify_Documents')
+    print('Creating Word Document...')
+
+    file_pathway = new_folder_path+f'/{date}.docx'
+    try:
+        os.mkdir(new_folder_path)  # Create the new folder
+
+    except FileExistsError:
+        pass  # Folder already exists
+        
+    try:
         document = docx.Document(file_pathway)
+    except:
+        document = docx.Document()
+    
     header_text = f'Voicemail Number {voicemailCount}:\n\n'
     document.add_heading(header_text, level=1)
     voicemailCount +=1
     document.add_paragraph(f"{response}\n\n")
     document.add_heading(f'\t\t\t\t\tTranscription:', level=2)
     document.add_paragraph(f"\n{transcript}\n\n")
-    document.save(file_pathway)  # how would i do this for clients?
+    document.save(file_pathway)  
 
 
 '''------------------------------------------------------------------------------------------------------'''
 
 def extract_audio_from_eml(part):
     # Get the 'parts' from the Gmail message
     current = part['parts']
@@ -355,21 +402,34 @@
     else:
         print("Converting Voicemail into audio file...")
         # Use the MIME type to determine the file extension
         ext = mimetypes.guess_extension(mime)
         if ext is None:
             ext = f'.{formats}'
 
-        filename =os.path.abspath(f'voicemails') 
-        if not os.path.isdir(f'{filename}/{date}/'):
-            filename = os.path.join(filename,f'{date}')
+        if sys.platform.startswith('win'):
+            desktop_path = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
+        elif sys.platform.startswith('darwin') or sys.platform.startswith('linux'):
+            desktop_path = os.path.join(os.path.expanduser("~"), "Desktop")
+        else:
+            raise Exception("Unknown operating system.")
+        new_folder_path = os.path.join(desktop_path, 'Linguify_Voicemails')
+        try:
+        # Create the new folder
+            os.mkdir(new_folder_path)
+            
+
+        except FileExistsError: 
+            pass
+        if not os.path.isdir(f'{new_folder_path}/{date}/'):
+            filename = os.path.join(new_folder_path,f'{date}')
             os.mkdir(filename)
             filename = os.path.abspath(filename)+f'/{voicemailCount}{ext}'
         else:
-            filename = filename+f'/{date}/{voicemailCount}{ext}'
+            filename = f'{new_folder_path}/{date}/{voicemailCount}{ext}'
         with open(filename, "wb") as attachment_file:
             attachment_file.write(ready_attachment_data)
 
         # Process the voicemail attachment
         print('AI Processing audio file...')
         process_audio_file(filename)
             
@@ -417,16 +477,16 @@
         # Search for voicemail emails
         print("Searching through emails for New Voicemails...")
         results = service.users().messages().list(         # Number of emails available
             userId='me', q='is:unread subject:"Voicemail"'
         ).execute()
 
         messages = results.get('messages', []) # Number of voicemails available
+        voice_processed = False
         if messages:
-            voice_processed = False
             for message in messages:
                 msg = service.users().messages().get(userId='me', id=message['id']).execute()  # for part in msg['payload']['parts']
                 for part in msg['payload']['parts']:
                     voicemail_content,mime_type,format = process_email_attachment(part, service,msg, True)
                     if voicemail_content != None:
 
                         # Mark the email as read
@@ -451,24 +511,24 @@
                     voicemailCount+=1
                     voice_processed = True
                     
 
                 except KeyError:
                     pass
                     
-        if voicemailCount == 1:
-            print('There are no New Voicemails!')  # Incase there's an email with voicemail as subject but no voicemail attachments
 
         if voice_processed:
             send_email_notification(credentials_file_path,company,voicemailCount-1)
         else:
             print('There are no New Voicemails!')
             
     except Exception as e:
         print(f"Error occurred: {e}\nPlease contact the provider (abdul_khafagy2004@hotmail.com).\n")
 
 '''------------------------------------------------------------------------------------------------------'''
 
 
-if __name__ == "__main__":
-    start()
-    
+start()
+"""python3 setup.py sdist bdist_wheel
+pip install .
+linguify
+"""
```

### Comparing `Linguify-1/setup.py` & `Linguify-2.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Linguify',
-    version=1,
+    version='2.0.0',
     packages=find_packages(),
+    package_data={'linguify': ['credentials.json']},
     install_requires=[
     "openai",
     "python-docx",
     "google-api-python-client",
     "google-auth-httplib2",
     "google-auth-oauthlib",
     "click"
     ],
-    entry_points={
-        'console_scripts': [
-            'linguify=linguify:start',
-        ],},
+    entry_points={"console_scripts": ["linguify=linguify:start"]},
+
     author='Abdulrahman Khafagy',
     author_email='abdul_khafagy2004@hotmail.com',
     description='Linguify is designed to automate voicemail transcription via email parsing.',
 )
+
+
```

