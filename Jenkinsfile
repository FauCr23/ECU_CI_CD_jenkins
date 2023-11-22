pipeline {
    agent any

    //environment {
    //    PLATFORMIO_HOME = 'C:\\Users\\danny\\OneDrive\\Documents\\PlatformIO\\Projects\\Test_hardware'
    //}

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/FauCr23/ECU_CI_CD_jenkins.git'
            }
        }
        stage('Build') {
            steps {
                bat 'echo System testing started...'
            }
        }
        stage('Test') {
            steps {
                bat 'pio test -vvv 
                //-d, --project-dir C:\\Users\\faust\\Documents\\PlatformIO\\Projects\\Test_Gateway'
            }
        }
    }
}
