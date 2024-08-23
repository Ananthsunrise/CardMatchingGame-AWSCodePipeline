**CardMatching Game through AWS CodePipeline**

In this project, We make card matching game using s3 static website. By using AWSCodepipeline automatically copy the files from github to s3bucket and make updates if any changes you want.


Procedure : 

Step1 : 
Setup your github repo.
You can form my github repository to get all files needed.  **CardMatchingGame-AWSCodePipeline**

Step 2 :
Make static website using s3
Go to s3->create 1 bucket->Disable block all public access ->add buckey policy by paste the attched code in this repo-> enable static website hosting

Step3:
Create codepipeline to automate process
Go to codepipeline->create pipeline->select source provider ar github and select your repo->skip buildprovider->select deploy provide as your s3 bucket
Now your pipeline is successfully created.

Copy your statci website link from s3 and put in new tab. Your game is ready!!

Step 4:
If you want make change in your game, you need to update files in your github repo. Then codepipeline automatically update your changes
