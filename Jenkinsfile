pipeline {
  agent {
    docker {
      args '-v /root/.m2:/root/.m2'
      image 'jenkins-agent-maven-35-rhel7'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }

  }
}