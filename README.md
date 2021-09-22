# monai2021bootcamp-aws-instructions

These setup instructions describe how to access the AWS accounts for the third day of the [MONAI MICCAI Bootcamp 2021](https://gpuhackathons.org/event/monai-miccai-bootcamp-2021). Each account will be shared by two users and every user will launch a dedicated GPU-based SageMaker notebook instance to work on the ML challenges. 


## Accessing your AWS account

* Go to https://dashboard.eventengine.run/login and enter the event hash you have received via email and click on **Accept Terms & Login**:

![image](https://user-images.githubusercontent.com/611112/134424302-d4cd964d-e77a-4d44-bcf5-54d623694454.png)

* On the next page, click on **Email One-Time Password (OTP)**:

![image](https://user-images.githubusercontent.com/611112/134424689-145d499e-7788-4933-807a-36bf633e5d51.png)

* Enter the email address, which you used when you registered for the bootcamp an 

![image](https://user-images.githubusercontent.com/611112/134425434-5ac86a21-4c63-4adb-b144-dfaa457a090a.png)

* In the next window, click on **AWS Console**:

![image](https://user-images.githubusercontent.com/611112/134418929-dc458dda-c3dc-4990-8c48-7f9c4b39340b.png)

* Another window will open. Please click on **Open AWS Console**:

![image](https://user-images.githubusercontent.com/611112/134417890-13ba1ba7-c090-4fa6-bbfa-8a5472381228.png)

* Congratulations, you have accessed your AWS account, which you will use for the rest of the day. Now, we need to make sure to launch your own Jupyter server.

## Launching your pre-configured SageMaker Notebook instance 

* In the search bar on the top, please type "service catalog" and click on **Service Catalog** in the search result list:

![image](https://user-images.githubusercontent.com/611112/134418466-e7b68b3d-3120-4257-9349-9b32f666ce1e.png)

* In Service Catalog, click on **Bootcamp Notebook**:

![image](https://user-images.githubusercontent.com/611112/134418833-90bea6f3-1462-4d99-8e4f-f07da776b225.png)

* Click on **Launch product**:

![image](https://user-images.githubusercontent.com/611112/134419214-c6b12074-f91c-4ff8-9227-daa82c3fc439.png)

* Enter your specific notebook name into the **Provisioned product name** field and the **NotebookInstanceName** field. Remember, two users will share the same AWS account. Therefore, we recommend using a naming schema like `notebook-[firstnamelastname]`. After that, click on **Launch product** at the bottom. This will launch your pre-configured GPU-based SageMaker Jupyter notebook server in the background. 

![image](https://user-images.githubusercontent.com/611112/134419557-46ee3d2d-94a6-43a2-a0f9-79aa6f765918.png)

* Now, we can leave Service Catalog.In the search bar at the top, enter "sagemaker" and click on **SageMaker** in the search result list:

![image](https://user-images.githubusercontent.com/611112/134420293-4bacd492-9505-483b-90c8-fadce095912f.png)

* In the SageMaker Console, click on **Notebook instances** in the left sidebar:

![image](https://user-images.githubusercontent.com/611112/134420704-5ec5face-e098-4474-921a-c619cb6a1997.png)

* In the list of notebook instances, you will see the instance you just started via service catalog. If your instance is not yet in status "InService", just wait 1-2 minutes until the server was completely launched. Click on **Open Jupyter Lab**, which will open your Jupyter Lab environment in a separate tab. 
 
![image](https://user-images.githubusercontent.com/611112/134421324-34b9edf2-5169-406e-af1a-c5050ce92c4e.png)

## Downloading the bootcamp notebooks

* In Jupyter Lab, click on **File > New > Terminal**. We will now git clone the notebooks for today's challenge day. 

![image](https://user-images.githubusercontent.com/611112/134421836-1ff822cc-1369-42ff-9d4e-828f9da5ad61.png)

* In the terminal, type `cd SageMaker` and press **Enter**. Then type `https://github.com/zephyrie/bootcamp_test` and press **Enter** again. After that, you will be able to navigate to the notebooks you just downloaded via the file browser on the left

![image](https://user-images.githubusercontent.com/611112/134422614-4c74ab74-cc95-44ac-853a-8027df8daf11.png)

## Launching Juypter notebooks

**Important**: When selecting and launching a notebook, you will be asked to select your preferred kernel. Please make sure to always select the `conda_pytorch-latest_p36 kernel`:

![image](https://user-images.githubusercontent.com/611112/134423773-4b5983c5-a631-44d2-bade-3a302e19f733.png)





