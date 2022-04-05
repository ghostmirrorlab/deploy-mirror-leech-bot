# deploy-mirror-leech-bot

## Requirements

- Telegram Account
- Heroku Account
- Github Account
- Install Python on Windows
- Google Drive Account

## Repo Link: [Here](https://github.com/anasty17/mirror-leech-telegram-bot)

Now first thing first, fork the repo.

![image](https://user-images.githubusercontent.com/77688759/161710615-c450b852-6acc-481b-a84f-5b3d054b6b05.png)

Now download that repo to your pc.

![image](https://user-images.githubusercontent.com/77688759/161710894-b2840ddf-c186-4a9f-bcb0-e301ffd2d253.png)

the downloaded repo will be in zip file, extract it.

## Step 1: Create credentials.json

<details>
  
  <summary>Click Here</summary>
  
goto your google cloud console. [Here](https://console.cloud.google.com)
create a new project (if you already have a project then no need to create another one)

![image](https://user-images.githubusercontent.com/77688759/161712563-4a2e83ab-b2ba-4134-8d92-cef8e2c09af2.png)
![image](https://user-images.githubusercontent.com/77688759/161712650-1f2b0f7b-0a74-4527-a699-3e09feea2d3a.png)

now select the project you just create.

![image](https://user-images.githubusercontent.com/77688759/161712843-6c725354-c795-45d2-a008-6399d30df46b.png)
![image](https://user-images.githubusercontent.com/77688759/161712899-18bfe7d8-1454-483e-8d09-73bb2959b47e.png)

now search for drive api and enable it.

![image](https://user-images.githubusercontent.com/77688759/161713016-ebf934d5-e0a4-45b2-80f1-229f655feddb.png)
![image](https://user-images.githubusercontent.com/77688759/161713088-518e509c-340a-4786-9bd2-2d079e461f31.png)
![image](https://user-images.githubusercontent.com/77688759/161713346-688ebc8c-7335-4de8-8f6c-3ce75dc6a06b.png)

after enabling drive api
goto your oauth sonsent screen

![image](https://user-images.githubusercontent.com/77688759/161714067-b246af4e-d537-43cd-9604-88fc04c457a6.png)
![image](https://user-images.githubusercontent.com/77688759/161714348-7329c817-a7b3-40b3-b8b1-a51df465aae7.png)
![image](https://user-images.githubusercontent.com/77688759/161714421-3f64cc16-b1e3-4078-abdb-0f58e4a81113.png)
![image](https://user-images.githubusercontent.com/77688759/161714503-5d7cd60b-2a29-4b19-83c1-e409ebf22639.png)
![image](https://user-images.githubusercontent.com/77688759/161714557-6e35f134-fd76-4f3b-a22f-84df9b201c5f.png)
![image](https://user-images.githubusercontent.com/77688759/161714611-b6a066e0-820c-48f4-8591-90cbcc8774d0.png)
![image](https://user-images.githubusercontent.com/77688759/161714665-9acaf68f-a9de-4ab7-8e7f-e64d8db81cb1.png)
![image](https://user-images.githubusercontent.com/77688759/161714725-63cc7c7b-0473-4d47-b7a4-545a8eae1c8b.png)
![image](https://user-images.githubusercontent.com/77688759/161715003-997b25af-53d8-43a4-a25f-171ee4c0d50b.png)
![image](https://user-images.githubusercontent.com/77688759/161715060-4107aa1c-8f79-4e14-bcda-5c7dd7355892.png)
![image](https://user-images.githubusercontent.com/77688759/161715135-b6ccae58-eb01-40dd-989a-9b85df56e9dd.png)
![image](https://user-images.githubusercontent.com/77688759/161715506-734544a8-38d6-41fc-89a3-6ea25ee03e52.png)
![image](https://user-images.githubusercontent.com/77688759/161715635-5a915180-18b7-4487-b3d7-d9683c65d599.png)
![image](https://user-images.githubusercontent.com/77688759/161715762-dad89c26-6b64-46c6-a5ac-9eac373658cc.png)

and done now download your .json file 

![image](https://user-images.githubusercontent.com/77688759/161715944-34b24641-a2b9-4236-8f97-b1a292e5e3e5.png)

after download rename it to `credentials.json`
Now move that credentials.json file to the extracted repo folder

![image](https://user-images.githubusercontent.com/77688759/161720299-4ee43d15-f136-41e0-b5f7-2bb822429999.png)

we are done with the credentials.json file.

</details>
  
## Step 2: Create token.pickel

<details>
  
  <summary>Click Here</summary>
  
for genrating token.pickel you will need python
so install python from this link [Here](https://www.python.org/downloads/)
while installing, make sure thagt `add to the path` option is selected.
onced installed, open cmd and type `python --version` to make that you have installed python correctly.
  
![image](https://user-images.githubusercontent.com/77688759/161721207-223e78f8-d9dc-4b76-9314-0fe76d5bc109.png)

ok, now goto your extracted folder click on the address bar and type cmd then hit enter.
  
![image](https://user-images.githubusercontent.com/77688759/161721454-52142434-4f3e-44b5-a3f5-7f0fd9b4f03f.png)
![image](https://user-images.githubusercontent.com/77688759/161721551-cf5d24b4-b518-4245-997b-a5b72409ed1e.png)
![image](https://user-images.githubusercontent.com/77688759/161721614-1a1af809-229c-49df-9f85-64f33debd543.png)

there you go.
now give command
`pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib`

now make sure to set a default browser, in my case chrome is the default.

then run
`python generate_drive_token.py`

one browser window will open the follow the on screen prompt
  
![image](https://user-images.githubusercontent.com/77688759/161724909-723eac9b-3caa-46bf-803c-4dd0c42b3642.png)
![image](https://user-images.githubusercontent.com/77688759/161724965-ba3068e6-720e-4331-9b71-a890cb8e8731.png)
![image](https://user-images.githubusercontent.com/77688759/161725004-91f84911-ea58-426e-a0d4-ea28db5dc54b.png)
![image](https://user-images.githubusercontent.com/77688759/161725045-d16bcb9c-1f4b-49e0-a18e-af7e6dc66103.png)

now after you reach this screen 
  
![image](https://user-images.githubusercontent.com/77688759/161725108-78da920f-70f8-4f46-9cb7-b2015651cfcf.png)

token.pickel will be available in the ectracted repo folder
  
![image](https://user-images.githubusercontent.com/77688759/161725413-bfd6dc6f-2d0c-4668-98ba-525d73467c65.png)

</details>  

## Step 3: Hosting token.pickel

<details>
  
  <summary>Click Here</summary>
  
now we need to host our token.pickel and credentials.json 
for that we will be going to use index.

we will use this [repo](https://gitlab.com/ParveenBhadooOfficial/Google-Drive-Index) for our hosting.
go to [this](https://bdi-generator.hashhackers.com/) site 

![image](https://user-images.githubusercontent.com/77688759/161735755-06598ea0-0683-4a46-932c-02f1047721cb.png)

sign in to get the Authentication Code

![image](https://user-images.githubusercontent.com/77688759/161735885-5fd3e64b-9e1b-4b0e-99d0-2b045055d13b.png)
![image](https://user-images.githubusercontent.com/77688759/161735955-afaad737-526c-4d3d-81c8-aa3eee18dc9d.png)
![image](https://user-images.githubusercontent.com/77688759/161736007-c3719cd2-0669-4eba-9632-573b4a4f6138.png)

paste that code in `Authentication Code`

![image](https://user-images.githubusercontent.com/77688759/161736264-f68a9e54-e495-4a16-aaea-351334164ff0.png)

for `Site Name` you can give any for eg `personal`
for `Share Drive ID or root` goto your drive and create a new folder for your index (dont create this folder in shared drive you created previously)

![image](https://user-images.githubusercontent.com/77688759/161736709-0adeca7d-f0d1-4caf-813a-a320822bdfe4.png)

go inside that folder and copy the id of that folder

![image](https://user-images.githubusercontent.com/77688759/161736798-f24dda46-9f26-4724-bdcf-3601a19c70ba.png)

use it for `Share Drive ID or root`

![image](https://user-images.githubusercontent.com/77688759/161736899-c38cfa61-e55f-423e-a747-d169f6d31eab.png)

then click on submit and copy the genrated for your index 

![image](https://user-images.githubusercontent.com/77688759/161737009-ea620aef-7e44-436a-b84e-d6d5e6143daa.png)

now goto [cloudflare](https://www.cloudflare.com/) and sign up for an account.

then goto  `workers`

![image](https://user-images.githubusercontent.com/77688759/161737351-e2324694-a145-4a14-850b-43f3e718d024.png)
![image](https://user-images.githubusercontent.com/77688759/161737457-28bedba5-5e0b-4c53-84d9-89629a0467a6.png)
![image](https://user-images.githubusercontent.com/77688759/161737508-e8021e09-89ef-4da9-bb5e-1e8b2a58a6dc.png)

then complete the verification process and come back to the `workers` section again.

![image](https://user-images.githubusercontent.com/77688759/161737755-d5475d08-0b2d-4b32-8b63-a6c57674f7b6.png)
![image](https://user-images.githubusercontent.com/77688759/161737848-9cbc23d0-edeb-424c-a9e5-73bbb8480b23.png)
![image](https://user-images.githubusercontent.com/77688759/161737948-9c5f1dc2-5a81-4e71-8721-de03fe813b99.png)

remove all the content from here

![image](https://user-images.githubusercontent.com/77688759/161738144-1f6c94c6-7753-459d-8fe3-0ceb2d60ece0.png)

and paste the code u genrated for your index then click on `save and deploy`

![image](https://user-images.githubusercontent.com/77688759/161738371-a344f75a-da78-49a3-ac30-2bd886df9b50.png)
![image](https://user-images.githubusercontent.com/77688759/161738430-03e9d198-c810-457c-8315-db54b900b5c3.png)

now wait for 10 seconds your index will be online.

save the link for your index

![image](https://user-images.githubusercontent.com/77688759/161738546-de13a74a-36cf-4949-b13e-74a650681f8f.png)

now goto that drive folder u create for the index and upload your token.pickel.

![image](https://user-images.githubusercontent.com/77688759/161742717-3864b06b-8715-4799-bf77-7267bef39725.png)

then open your index link click on `drive one` you will see your files u just uploaded.

![image](https://user-images.githubusercontent.com/77688759/161739501-b250a124-5d75-45f2-8b5b-e10091cb7635.png)
![image](https://user-images.githubusercontent.com/77688759/161742804-90ebd60c-1f4f-48ff-8b99-7755a9fc2ffc.png)


and done we successfully hosted our token.pickel in your index. (just dont share your index link)

  </details>

## Step 4: Create config.env

<details>
  
  <summary>Click Here</summary>
  
go [here](https://github.com/anasty17/mirror-leech-telegram-bot/raw/master/config_sample.env) and copy all the content.
then goto [github gist](https://gist.github.com/)

give your gist a name `config.env`

![image](https://user-images.githubusercontent.com/77688759/161727093-6bac51cf-f26d-46e7-950b-f85700b71be5.png)

and paste the previously copied content here

![image](https://user-images.githubusercontent.com/77688759/161727191-4f5038e8-aaee-49f4-bba7-cbe849386853.png)

now remove line no 2. `_____REMOVE_THIS_LINE_____=True`
then start filling the config values

for now i will only show the necessary values for the proper working of the mirror leech bot.

### BOT_TOKEN:
search @BotFather on telegram, start the bot and type `/newbot` then follow on the in screen instruction to create a new bot.

![image](https://user-images.githubusercontent.com/77688759/161728194-f12dd4e5-dab2-426d-a8af-b672ac7d3f69.png)

this will be your BOT_TOKEN

  
### GDRIVE_FOLDER_ID:
search @MSGuite_SD_Creator_Bot on telegram, start the bot click on `genrate td` now send your email address, give your drive a good name for eg `hitesh920's drive` and done.

![image](https://user-images.githubusercontent.com/77688759/161728959-fa766198-0e34-4d4d-bd51-f30f357d7d78.png)

now click here to go to your shared drive you just created.
now copy the root id of your shared drive
for eg https://drive.google.com/drive/folders/xxxxxxxxxxx then the code after `folders/` will be the your root id

![image](https://user-images.githubusercontent.com/77688759/161729686-d9e79a8f-4479-46ae-84dc-1989df4c75f9.png)

this will be the value of GDRIVE_FOLDER_ID 

  
### OWNER_ID:
search @MissRose_bot on telegram, start the bot then type `/id` bot will send your account's id
use that for OWNER_ID

  
### DOWNLOAD_DIR:
keep the default values, no need to change anything here.

  
### DOWNLOAD_STATUS_UPDATE_INTERVAL:
keep the default values, no need to change anything here.

  
### AUTO_DELETE_MESSAGE_DURATION:
keep the default values, no need to change anything here.

  
### IS_TEAM_DRIVE:
set the to `True` as we are using shared drive.

  
### TELEGRAM_API & TELEGRAM_HASH:
got [here](my.telegram.org) register with your number connected to telegram account fill with your number , choose desktop,  fill app title and short name to any name you want.

![image](https://user-images.githubusercontent.com/77688759/161731080-bff37137-e53a-4774-a1bd-6288491ca494.png)

this will give the values of `TELEGRAM_API` and `TELEGRAM_HASH`

<b>App api_id</b> will be your TELEGRAM_API and <b>App api_hash</b> TELEGRAM_HASH

### TOKEN_PICKLE_URL:
go to your index link and click on the token.pickel u just hosted in step 3 and copy the direct download link.
  
![image](https://user-images.githubusercontent.com/77688759/161749786-d71ab726-51b9-49b7-9dae-b584cd3177e2.png)

and use the url for TOKEN_PICKLE_URL

we are done with the all necessary configs for the proper working of the mirror leech bot.
it should look like this after filling all the necessary values
  
![image](https://user-images.githubusercontent.com/77688759/161732551-fe9424b4-d141-481c-9de3-d0cb368c1c96.png)

and we are done with all the necessary configs needed.
then click on create secret gist to save the gist.
  
![image](https://user-images.githubusercontent.com/77688759/161732712-6c3741ac-494b-496d-8fea-3ae21fc8ef3f.png)
  
we have successfully created our config.env
  
</details>
  
## Step 5: Setting Up Secrets For Github Action

<details>
  
  <summary>Click Here</summary>
  
goto your forked repo > settings > secrets > action

![image](https://user-images.githubusercontent.com/77688759/161750596-e539db44-2a42-4ac9-bc0d-b593777f84ee.png)
![image](https://user-images.githubusercontent.com/77688759/161753272-ddad44c9-2c98-40d0-b06a-67027ab222dd.png)

now here under secrets, you need to create 4 secrets 
- HEROKU_EMAIL
- HEROKU_API_KEY
- HEROKU_APP_NAME
- CONFIG_FILE_URL

![image](https://user-images.githubusercontent.com/77688759/161753685-a8e1da3a-8647-4f71-8221-b8d83c9977d8.png)
![image](https://user-images.githubusercontent.com/77688759/161753909-6b6c8c59-7d8a-4920-88e4-53d212099efe.png)

<b>Do the same for other three secrets.</b>

### HEROKU_API_KEY
goto your heroku account settings [Here](https://dashboard.heroku.com/account)

scroll down and copy thr api key

![image](https://user-images.githubusercontent.com/77688759/161752797-4a3c4798-352e-4c33-af23-ac0b5b9af3bf.png)

### HEROKU_APP_NAME:
name you would like to give to your heroku apps (must be unique)

### CONFIG_FILE_URL:
goto that gist you created for the config.env

then click on raw
  
![image](https://user-images.githubusercontent.com/77688759/161732830-d9489120-9d3c-4f74-8619-8c1fb94b8478.png)

and copy the url then remove the commit id

for eg `https://gist.githubusercontent.com/ghostmirrorlab/f9b1e6xxxxxxxxxxxxxaaac04520/raw/200d4a93e0eb5ee8d4b0e5a377ce0396a131843e/config.env` then the commit id will the one after `raw/` and before `/config.env`


`original config.env url`: https://gist.githubusercontent.com/ghostmirrorlab/f9b1e6xxxxxxxxxxxxxaaac04520/raw/200d4a93e0eb5ee8d4b0e5a377ce0396a131843e/config.env

`url after removing commit id`: https://gist.githubusercontent.com/ghostmirrorlab/f9b1e6xxxxxxxxxxxxxaaac04520/raw/config.env

now after removing the commit id use that url for the CONFIG_FILE_URL

once all the four secrets have been added, it should look like this

![image](https://user-images.githubusercontent.com/77688759/161755355-afcda2b7-3fb1-4e52-8876-162932213e40.png)

and we are done with the secrets.
  
</details>  

## Step 5: Deploy Bot
