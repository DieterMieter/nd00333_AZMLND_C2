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



## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
