pipeline {
    agent any
    environment{
          USERNAME='racha10r@gmail.com'
          ACCESS_KEY='iHnnmi0atXDjDKIqckdBH0gU72Uf8zJb76EyNlXjzvGPzvr54'
          TUNNEL=true
        }
    parameters {
        string(name: 'git', defaultValue: "CICD")
        string(name: 'test', defaultValue: "deploy")
    }

    stages {
        stage('connect to github') {
            steps {
                echo "${params.git}"
            }
        }
        stage('git-clone') {
            steps {
                echo 'user name is : ' env.USERNAME
                echo 'your access key is : 'env.ACCESS_KEY
                echo 'your tunnel are : 'env.TUNNEL
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
                echo "${params.test}"
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
