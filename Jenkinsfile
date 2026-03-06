pipeline {
    agent any
    stages {
        stage("Install") {
            steps {
              bat 'pnpm i'
              echo 'install success'
            }
        }
        stage("Build") {
            steps {
              bat 'pnpm build'
              echo 'build success'
            }
        }
        stage("Test") {
            steps {
                bat 'pnpm test:unit'
                bat 'pnpm test:e2e'
                echo 'test success'
            }
        }
        stage("Deploy") {
            steps {
                echo 'deploy success'
            }
        }
    }
}