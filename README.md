# flask_5_tailwind


## objective:

### The objective of this assigment was to provide hands-on experience in video hosting, creating a Flask app styled with Tailwind CSS, and deploying it to a cloud platform. We were to leverage CDN services in Google Cloud or Azure to optimize video delivery, ensuring a seamless user experience for viewers worldwide.

## objective 1: video creation and procurement

### 1. go to microsoft azure and search for "storage accounts" then click on it then make a storage account called "videoflask"



## objective 2: cloud cdn and video hosting

### 1. go to "data storage," click "containers" and upload a 10 second video that was created via zoom 

### 2. go to "security + networking" and click "front door and cdn" then configure an endpoint

### 3. copy the endpoint hostname and paste it into the tab

### 4. go back to "containers" in "storage accounts" and click on the video that you uploaded then copy the url into a new tab then copy everything after the .net

### 5. combine the copied part of the video url link with the endpoint hostname link 

### link: https://steph-test.azureedge.net/week5hw/week5hw.mp4



## objective 3: flask app deployment

### 1. cd into your repo

### 2. use the command curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash

### 3. run the following:

#### - python app.py to get a preview of the website

#### - az 

#### - az login --use-device-code then copy the code shown and click the link provided which will open a new tab where you can paste the code that you copied

#### - az webapp up --resource-group <groupname> --name <app-name> --runtime <PYTHON:3.9> --sku <B1> but replace <groupname> with the name of your resource group and <appname> with the name of your app. here is what it should look like: az webapp up --resource-group steph5042023 --name StephaniesCDNApp --runtime "PYTHON|3.9" --sku B1

### 4. go to "app services" on azure and click on the link for your app



## app link: stephaniescdnapp.azurewebsites.net



## observations and benefits of using a CDN and cloud deployment:

### cdns deliver web content to end-users more efficiently, reduce the latency and improve loading times which provide a faster user experience

### in addition to being faster, cdns are more tailored to wherever the user is on the planet

### cdns distribute traffic across multiple servers which help availability of web applicatioons

### cloud deployment allow for rapid increase or decrease of resources which ensure that your application can handle spikes in traffic

### cloud deployment allows for high availability which minimizes downtume and service interruptions


## challenges:

### there were no significant challenges when running this app