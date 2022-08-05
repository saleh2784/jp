pipeline {
    agent any
    environment{
          USERNAME='racha10r@gmail.com'
          ACCESS_KEY='iHnnmi0atXDjDKIqckdBH0gU72Uf8zJb76EyNlXjzvGPzvr54'
          TUNNEL=true
          test='deploy'
        }
    parameters {
        string(name: 'git', defaultValue: "CICD")
        choice (name: 'pool', choices: ['CI', 'Test', 'CD'], )
    }

    stages {
        stage('connect to github') {
            steps {
                echo "${params.git}"
            }
        }
        stage('git-clone') {
            steps {
                echo env.USERNAME
                echo env.ACCESS_KEY
                echo env.TUNNEL
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
                echo env.test
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
