
# Build and push Docker Image to AWS ECR

Here we will be adding to the jenkins pipeline, the code for docker build creating a docker image and pushing it to AWS Elastic Container Registry(ECR)

#### 1. Create Docker login credentials in jenkins

Jenkins Dashboard -> Manage Jenkins -> credentials -> Stores -> scoped to Jenkins -> System -> Global credentials -> Add credentials

Please note we will be giving dockerhub credentials.

![dockerhub](Picture1.png)

#### 2. Create AWS ECR 

AWS Dashboard -> Elastic Container Registry -> Get Started(Create Repository) -> Private-> RepositoryName -> Create Repository
RepositoryName = easyuggyapp

![ecr](Picture2.png)

![ecr](Picture3.png)

#### 3. Create AWS credentials in Jenkins

Jenkins Dashboard -> Manage Jenkins -> credentials -> Stores -> scoped to Jenkins -> System -> Global credentials -> Add credentials

![aws](Picture4.png)

![aws](Picture5.png)

The Access ID and secret key here will be your AWS access id and secret key.

#### 4. Jenkins file

Add stages to the existing Jenkins file

![jenkinsfile](Picture6.png)

#### 5. Create the pipeline job and configure

#### 6. Build the job

![log](Picture7.png)

#### 7. Validate ECR

![ecr](Picture8.png)



