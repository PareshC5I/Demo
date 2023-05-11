**Simple Sentiment Analysis Streamlit App**
This GitHub repository contains sentiment analysis app and all the required files for deploying it to AWS Beanstalk. By simply inputting the text into the app and clicking "Analyze," users can quickly receive an overview of the positive, negative, and neutral sentiment within the text. Below is the logical architecture diagram and explanation. 
![MicrosoftTeams-image](https://github.com/PareshC5I/Demo/assets/101194021/ca6c5f41-dbbe-445d-957e-e969c4573f24)
Steps
- Pushing all the required files along with app.py, Dockerfile, requirements.txt and Dockerrun.aws.json from local to GitHub repository (PareshC5I/Demo).
  - app.py - Have the streamlit app
  - Dockerfile - For creating and running the image
  - requirements.txt - Have all the required libraries
  - Dockerrun.aws.json - For Beanstalk to pull the image 
- Created yml file for CI/CD using GitHub actions.
- Created the application and environment in AWS Elastic Beanstalk. 
- Saving all the necessary credentials to GitHub secrets.
- Run yml file for building and pushing the docker image to dockerhub then zip all the files together and then deploy it to AWS Elastic Beanstalk.
- Use the URL generated from AWS Elastic Beanstalk to access the Streamlit App
Making or pushing any changes to the GitHub runs the yml file and the AWS Elastic Beanstalk URL is updated.

