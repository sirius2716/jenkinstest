pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'mvn --version'
      }
    }

    stage('Print') {
      steps {
        echo 'Halih�'
        sh 'uname -a | tee os.txt'
        archiveArtifacts 'os.txt'
      }
    }

  }
}