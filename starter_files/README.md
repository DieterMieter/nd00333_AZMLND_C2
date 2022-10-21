# Machine Learning Engineer with Microsoft Azure: Project 2
## Operationalizing Machine Learning
In this project I used AzureML Studio to create, deploy and consume a machine learning model as well as a pipeline.

## Architectural Diagram
![image](https://user-images.githubusercontent.com/115837790/197182994-4558df25-a888-49b2-9afc-bebeb5c5f09d.png)
This Image from the Task description gives an architectural overview of the project:
1. Authentication: Not applicable when working in the given lab workspace
2. Auto ML model: Let AutoML select an appropriate model to return predictions on the BankMarketing Dataset
3. Deploy the best model: Deploy the model as a webservice, reachable through a REST API
4. Enable logging: Turn on application Insights to monitor the behavior of the endpoint
5. Consume model endpoints: Send a request to the endpoint through http, POST some data to return a prediction on
6. Create and publish a pipeline: Set up a way to efficiently retrain the model
7. Document a the steps with screenshots, a screencast and this Readme

## Key Steps
### Step2: Automated ML Experiment
Create Dataset from .csv file:
<img width="805" alt="Dataset" src="https://user-images.githubusercontent.com/115837790/197184792-3ffdb900-2d99-46ca-b32d-99af1f95a2bb.PNG">

AutoML experiment completed:
<img width="777" alt="Experiment-completed" src="https://user-images.githubusercontent.com/115837790/197184970-56a93da5-7f78-4a21-a4d4-5767a9731372.PNG">

Best model from AutoML:
<img width="776" alt="best-model" src="https://user-images.githubusercontent.com/115837790/197185018-b6c77490-0177-4d14-8245-33ed6fb1cb64.PNG">

### Step3: Deploy the Best Model
Best Model Deployed:
![image](https://user-images.githubusercontent.com/115837790/197185590-f4bf6791-48a9-48f7-805f-c84a88ca6bc5.png)

### Step4: Enable Logging
Application Insights enbaled for endpoint:
<img width="525" alt="App-Insights-enabled-new" src="https://user-images.githubusercontent.com/115837790/197185912-5c5a92d1-ffb5-423d-a0f3-e676aa71e43e.PNG">

Output of logs.py scripts:
<img width="371" alt="logs1" src="https://user-images.githubusercontent.com/115837790/197186006-55b3fa55-8ee5-4c21-a3e3-8d30f31f15ac.PNG">
<img width="374" alt="logs2" src="https://user-images.githubusercontent.com/115837790/197186018-7e6415ac-a51e-4caf-bac3-67b2038c930f.PNG">
<img width="371" alt="logs3" src="https://user-images.githubusercontent.com/115837790/197186040-5652ad2c-7bdd-42d1-ac74-194c6f4a2c37.PNG">
<img width="371" alt="logs4" src="https://user-images.githubusercontent.com/115837790/197186061-118ce0f4-e588-4576-a8bd-d0d41f23a21a.PNG">
<img width="372" alt="logs5" src="https://user-images.githubusercontent.com/115837790/197186070-7b249ded-b930-416f-85dd-9be0eb9e1b7a.PNG">
<img width="375" alt="logs6" src="https://user-images.githubusercontent.com/115837790/197186079-2a8a8fa9-d9a8-4beb-8893-50961b62af0f.PNG">
<img width="371" alt="logs7" src="https://user-images.githubusercontent.com/115837790/197186099-39d9bb13-267f-4120-bbf0-499dfb5eb0ba.PNG">
<img width="373" alt="logs8" src="https://user-images.githubusercontent.com/115837790/197186112-30640392-6071-4028-a176-468437d2d786.PNG">

### Step5: Swagger Documentation
Swagger on localhost with HTTP API methods and responses for the model:
<img width="773" alt="swagger-api1" src="https://user-images.githubusercontent.com/115837790/197186253-f0ea2e5f-94fd-41f6-b153-dab20ea945dd.PNG">
<img width="775" alt="swagger-api2" src="https://user-images.githubusercontent.com/115837790/197186265-90b1e197-372b-4fc7-85da-bd29735a124e.PNG">
<img width="774" alt="swagger-api3" src="https://user-images.githubusercontent.com/115837790/197186282-579aeebe-a453-4bcf-bc98-44207b37938a.PNG">
<img width="776" alt="swagger-api4" src="https://user-images.githubusercontent.com/115837790/197186290-115e2df4-c423-46b9-ace6-27b22a1458bb.PNG">
<img width="776" alt="swagger-api5" src="https://user-images.githubusercontent.com/115837790/197186302-f9a511b0-0fcb-4ef2-85ac-09a806bb47a5.PNG">

### Step6: Consume Model Endpoints
Check JSON output of model by running endpoint.py against the API:
<img width="529" alt="endpoint-py-output" src="https://user-images.githubusercontent.com/115837790/197186695-9e407643-e0e4-40f9-a434-bbd519fa9f33.PNG">

### Step7: Create, Publish and Consume a Pipeline
Pipeline has been created:
<img width="774" alt="pipeline-created" src="https://user-images.githubusercontent.com/115837790/197186832-0fe9dea9-f7f0-450d-9995-b057e8381fa3.PNG">

Pipeline Endpoint:
<img width="773" alt="pipeline-endpoint-new" src="https://user-images.githubusercontent.com/115837790/197186879-196c483b-64de-433e-b2aa-fc2d1794c0b2.PNG">

Bankmarketing Dataset with AutoML module:
<img width="774" alt="Bankmarketing-Dataset-with-AutoML-module" src="https://user-images.githubusercontent.com/115837790/197186973-42941b1c-6fbc-4ebe-a6f8-7c84cca24839.PNG">

Published Pipeline Overview showing REST endpoint and status of ACTIVE:
<img width="773" alt="published-pipeline-overview" src="https://user-images.githubusercontent.com/115837790/197187069-44860b05-7d73-4c44-8b2c-4827e9f9b7d3.PNG">

RunDetails Widget from Jupyter Notebook:
<img width="774" alt="run-details-widget" src="https://user-images.githubusercontent.com/115837790/197187169-c98a4aca-237e-46ff-829d-272f6f8ede31.PNG">

Scheduled run in ML Studio:
<img width="776" alt="Scheduled-run-2" src="https://user-images.githubusercontent.com/115837790/197187219-7c50613e-caa1-4502-aec4-cc327353c05d.PNG">

## Screen Recording
https://vimeo.com/762611422
