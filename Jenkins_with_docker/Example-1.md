
Ref: https://www.jenkins.io/doc/book/pipeline/docker/

#### Containerized builds

Step-1: Install Jenkins - refer: [JenkinsSetup](https://github.com/DevOpsOnlineTraining-2021/Jenkins/tree/master/JenkinsSetup)

Step-2: Configure Linux server to Jenkins master as Jenkins node and give the lable as 'dockerBuild'

Step-3: Install docker on Jenkins node - [Dokcer-Installation-Ubuntu](https://github.com/DevOpsOnlineTraining-2021/Docker/blob/main/DockerEngine/1.1.Dokcer-Installation-Ubuntu.md) or [Dokcer-Installation-AmazonLinux.md](https://github.com/DevOpsOnlineTraining-2021/Docker/blob/main/DockerEngine/1.3.Dokcer-Installation-AmazonLinux.md)

Step-3: Create pipeline job and update the job configuration with below snippet.

Step-4: Run the build

