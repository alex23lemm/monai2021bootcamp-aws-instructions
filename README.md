# monai2021bootcamp-aws-instructions

These setup instructions describe how to access the AWS accounts for the third day of the [MONAI MICCAI Bootcamp 2021](https://gpuhackathons.org/event/monai-miccai-bootcamp-2021). Each account will be shared by two users and every user will launch a dedicated GPU-based SageMaker notebook instance to work on the ML challenges. 


## Accessing your AWS account

* Go to https://dashboard.eventengine.run/login and enter the event hash you have received via email and click on **Accept Terms & Login**:

![image](https://user-images.githubusercontent.com/611112/134424302-d4cd964d-e77a-4d44-bcf5-54d623694454.png)

* On the next page, click on **Email One-Time Password (OTP)**:

![image](https://user-images.githubusercontent.com/611112/134424689-145d499e-7788-4933-807a-36bf633e5d51.png)

* Enter the email address, which you used when you registered for the bootcamp. Using another email address won't allow you to access your temporary AWS account.   

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

* Enter your specific notebook name into the **Provisioned product name** field and the **NotebookInstanceName** field.  Remember, two users will share the same AWS account. Therefore, we recommend using a naming schema like `notebook-[firstnamelastname]`. The name must start with a letter (A-Z, a-z) or number (0-9) and can include hyphens (-), but not spaces. After that, click on **Launch product** at the bottom of the page (The launch button is not shown in the screenshot below). This will launch your pre-configured GPU-based SageMaker Jupyter notebook server in the background. 

![image](https://user-images.githubusercontent.com/611112/134419557-46ee3d2d-94a6-43a2-a0f9-79aa6f765918.png)

* After that, you will see a notification on the top of the page that your notebook is being launched:

![image](https://user-images.githubusercontent.com/611112/134648396-2f8d384f-790c-4d5e-8447-5b244afcb109.png)

* Now, we can leave Service Catalog.In the search bar at the top, enter "sagemaker" and click on **SageMaker** in the search result list:

![image](https://user-images.githubusercontent.com/611112/134420293-4bacd492-9505-483b-90c8-fadce095912f.png)

* In the SageMaker Console, click on **Notebook instances** in the left sidebar:

![image](https://user-images.githubusercontent.com/611112/134420704-5ec5face-e098-4474-921a-c619cb6a1997.png)

* In the list of notebook instances, you will see the instance you just started via service catalog. If your instance is not yet in status "InService", just wait 1-2 minutes until the server was completely launched. Click on **Open Jupyter Lab**, which will open your Jupyter Lab environment in a separate tab. 
 
![image](https://user-images.githubusercontent.com/611112/134421324-34b9edf2-5169-406e-af1a-c5050ce92c4e.png)

## Downloading the bootcamp notebooks

* In Jupyter Lab, click on **File > New > Terminal**. We will now git clone the notebooks for today's challenge day. 

![image](https://user-images.githubusercontent.com/611112/134421836-1ff822cc-1369-42ff-9d4e-828f9da5ad61.png)

* In the terminal, type `cd SageMaker` and press **Enter**. Then type `git clone https://github.com/Project-MONAI/MONAIBootcamp2021` and press **Enter** again. After that, you will be able to navigate to the notebooks you just downloaded via the file browser on the left:

![image](https://user-images.githubusercontent.com/611112/134502649-760221b7-0d5f-4057-ba29-9279676d1c9d.png)

* Congratulations! You are now ready to get started. **The NVIDIA team will share specific information on the notebooks for the Bootcamp Challenge Day you will use today later during our intro session**. But please, keep on reading the last section below.  

## Launching Juypter notebooks

**Important**: When selecting and launching a notebook, you will be asked to select your preferred kernel. Please make sure to always select the `conda_pytorch-latest_p36 kernel`:

![image](https://user-images.githubusercontent.com/611112/134423773-4b5983c5-a631-44d2-bade-3a302e19f733.png)

**Have fun today and good luck with the mini challenges!**

## IMPORTANT: The notebooks were just updated on 4:45PM PT

If you downloaded the notebooks before, please make sure to run through the following instructions:

* In Jupyter Lab, click on File > New > Terminal. In the terminal, type `cd SageMaker` and press Enter. 
* Then type `git pull https://github.com/Project-MONAI/MONAIBootcamp2021` and press Enter again.

## Additional resources for another day
Below, we also added the links to the recourses, which were mentioned in the AWS on MONAI session on Day 2.  

### Basic AWS tutorials
* Launching a Deep Learning AMI: https://aws.amazon.com/getting-started/hands-on/train-deep-learning-model-aws-ec2-containers/ 
* Launching a Deep Learning Container: https://aws.amazon.com/getting-started/hands-on/get-started-dlami/ 
* SageMaker Technical Deep Dive Series: https://www.youtube.com/watch?v=uQc8Itd4UTs&list=PLhr1KZpdzukcOr_6j_zmSrvYnLUtgqsZz
 
### MONAI on SageMaker blog posts and repos
* Build a medical image analysis pipeline on Amazon SageMaker using the MONAI framework: https://aws.amazon.com/blogs/industries/build-a-medical-image-analysis-pipeline-on-amazon-sagemaker-using-the-monai-framework/
* GitHub repo: https://github.com/aws-samples/amazon-sagemaker-monai-examples
 
* Annotate DICOM images and build an ML model using the MONAI framework on Amazon SageMaker: https://aws.amazon.com/blogs/machine-learning/annotate-dicom-images-and-build-an-ml-model-using-the-monai-framework-on-amazon-sagemaker/
* GitHub repo: https://github.com/aws-samples/annotate-medical-images-in-dicom-server-and-build-ml-models-on-amazon-sagemaker
 
### ML-related Medical Imaging Challenges
* Grand-challenge: https://grand-challenge.org

### Misc
* MONAI dataset (Medical Segmentation Decathlon) on the Registry of Open Data: https://registry.opendata.aws/msd/


