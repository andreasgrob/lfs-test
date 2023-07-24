pipeline {
  agent {
    kubernetes {
      label 'hello-app'  // all your pods will be named with this prefix, followed by a unique id
      idleMinutes 2  // how long the pod will live after no jobs have run on it
    }
  }
  stages {
    stage('Hello Stage') {
      steps {
        sh "echo Hello !"
        sh "cat test.txt"
      }
    }
  }
}
