pipeline {
  agent any
  stages {
    stage('Checkout Scm') {
      steps {
        git 'https://github.com/2021Devops2019QxTeam/UsableCodes/'
      }
    }

    stage('Shell script 0') {
      steps {
        sh '''cd \'/var/lib/jenkins/workspace/DockerBuildProj/target\'
docker build -t dockerizedapp .
docker run -d -p 8085:8080 dockerizedapp'''
      }
    }

  }
}
