pipeline {
  agent any
    stages {
        stage('One') {
            steps {
                echo 'One output test'
            }
        }
        stage('Two') {
            steps {
                echo 'Could do something else here'
            }
        }
        stage('Three') {
            when {
                not {
                    branch "master"
                }
            }
            steps {
                echo "Hello"
            }
        }
    }
}
