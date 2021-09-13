
Ref: https://www.jenkins.io/doc/book/pipeline/docker/

#### Containerized builds

Step-1: Create One EC2 instance and then connect to it. Install Jenkins - refer: [JenkinsSetup](https://github.com/DevOpsOnlineTraining-2021/Jenkins/tree/master/JenkinsSetup)

Step-2: Create another EC2 instance and then connect to it. Install git and java.

Step-3: Configure Linux server to Jenkins master as Jenkins node and give the lable as 'dockerBuild'

Step-4: Install docker on Jenkins node - [Dokcer-Installation-Ubuntu](https://github.com/DevOpsOnlineTraining-2021/Docker/blob/main/DockerEngine/1.1.Dokcer-Installation-Ubuntu.md) or [Dokcer-Installation-AmazonLinux.md](https://github.com/DevOpsOnlineTraining-2021/Docker/blob/main/DockerEngine/1.3.Dokcer-Installation-AmazonLinux.md)

Step-5: Create pipeline job and update the job configuration with below git repo.

      Git repo URL: https://github.com/venkatasykam/DevOpsWebApp.git
      Git Branch: containerized-build
      Jenkins file: https://github.com/venkatasykam/DevOpsWebApp/blob/containerized-build/Jenkinsfile

Step-6: Execute the job and observer the build console output.

