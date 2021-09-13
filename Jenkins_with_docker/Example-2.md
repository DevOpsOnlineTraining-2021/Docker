
Step-1: Make sure jenkins and node configured - perform Step-1 to Step-3 from [Example-1](Example-1.md)

Step-2: Create a new pipeline job and add configure job with below script.

      pipeline {
          agent none
          stages {
              stage('Back-end') {
                  agent {
                      docker { image 'maven:3.8.1-adoptopenjdk-11' }
                  }
                  steps {
                      sh 'mvn --version'
                  }
              }
              stage('Front-end') {
                  agent {
                      docker { image 'node:14-alpine' }
                  }
                  steps {
                      sh 'node --version'
                  }
              }
          }
      }


Step-3: Execute the job and observer the build console output.
