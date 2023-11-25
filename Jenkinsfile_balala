pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                echo "Build App"
                sleep (5)
            }
        }
        stage ('Test') {
            parallel {
                stage('Test 1') {
                    steps {
                        echo "Test App 1"
                        sleep(10)
                    }
                }
                stage('Test 2') {
                    steps {
                        echo "Test App 2"
                        sleep(10)
                    }
                }
                stage('Test 3') {
                    steps {
                        echo "Test App 3"
                        sleep(10)
                    }
                }
            }
        }
        stage ('Deploy') {
            steps {
                echo "Deploy App"
            }
        }
    }
}
