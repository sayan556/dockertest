pipeline {
agent any
  stages {

    stage('image check'){
       steps{
          sh 'docker images'
        }
    }
    stage('image pull'){
       steps{
          sh 'docker pull nginx:latest'
        }
    }
    stage('dockerhub login'){
       steps{
          sh 'docker login -u sayan556 -p Sayanm15@'
        }
    }
    stage('image push'){
       steps{
          sh 'docker tag nginx sayan556/dock2:dockertest3'
          sh 'docker push sayan556/dock2:dockertest3'
        }
    }
  }
}
