pipeline {
    agent any

    stages {
        stage('connect to github') {
            steps {
                echo 'Hello World'
            }
        }
        stage('git-clone') {
            steps {
                echo 'the code are cloned'
                pwd()
            }
        }
        stage('build') {
            steps {
                echo 'bulding'
            }
        }
        stage('test') {
            steps {
                echo 'testind'
            }
        }
        stage('Debloy') {
            steps {
                echo 'deloyed'
                sh 'pwd'
                sh 'cat test.txt'
                
            }
        }
    }

}
