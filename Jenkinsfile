pipeline {
    agent any
     parameters {
        string(name: 'git', defaultValue: "Hello World")
        string(name: 'test', defaultValue: "done")
    }

    stages {
        stage('connect to github') {
            steps {
                echo ${params.git}
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
                echo ${parameters.test}
            }
        }
        stage('Debloy') {
            steps {
                echo 'deloyed'
                sh 'pwd'
                sh 'cat test.txt'
                sh 'touch 1.txt'
                
            }
        }
    }

}
