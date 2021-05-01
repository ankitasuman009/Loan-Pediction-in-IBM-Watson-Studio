# Loan-Pediction-in-IBM-Watson-Studio

# Prerequisites - 

Account in IBM Watson Cloud http://ibm.com/
Train dataset of Loan Eligibility https://www.kaggle.com/leonbora/analytics-vidhya-loan-prediction?select=train.csv


Steps to follow to make this model : 

1. Create a empty project. 
  ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img2.png)
  I named my project as "Aapno Bank".
2. Add assets from your local device. Asset here is your train dataset in .csv format.
  ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img3.png)
3. a) Once the file is uploaded, click Add to project and choose AutoAI experiment. AutoAI experiment is by default works on binary classification problem. So we don't have to make any changes here.
  ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img4.png)
  b) Name your experiment as 'AutoAI Experiment - Loan Prediction' and make sure you've selected a Machine Learning service instance. Once you associate your ML service, you can create your AutoAI experiment
  ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img5.png)
4. Choose Select From Project and choose the train.csv file you uploaded in your data assets.
  ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img6.png)
6. Select the target column for prediction which is Loan_Status. And then Run the Experiment. This will take few minutes.
  ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img7.png)
8. After this you can check which model is the best in Pipeline section. The first one with a star is the best to choose. Save that model with Save As option. Use the defalut name of this model and create it.
  ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img8.png)
10. a) Now you can go back to your project and will find this model under your assets section. 
    b) Click the three dots and promote this model.
    ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img9.png)
8. For this you need a Deployemnt space. You can either create a new one or can use the existing. I'm using the one I created Loan Eligibility Deployment Space. Then promote it.
   ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img10.png)
10. Now the deployment is done. Use the three lines of left panel and go to the deployment section. You can choose view all spaces if you can't find yours in the list.
11. a) Now use that flight symbol and deploy your model here.
     ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img11.png)
    b) Use online mode and give a name to your deployment. Create it.
    ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img12.png)
    c) Go to the deployemnt section, your deployemt will take if minutes to complete.
    d) Once completed, click on it. You'll direct a page and after that choose the deployment that we created just now.
11. Go to test section, put the values run it and see the result. The input should be provided in JSON form.
    ![img1](https://github.com/ankitasuman009/Loan-Pediction-in-IBM-Watson-Studio/blob/main/Images/img13.png)

Congratulations only if you completed this task. Thank You.
