pipeline {
    agent any
    stages
            {
                stage('docker-compose UP')
                        {
                            steps {
                                bat 'echo %PATH%'
                            }
                        }
                stage('Executing Tests')
                        {
                            steps {
                                echo "Testing the Project.........."
                            }
                        }
                stage('docker-compose DOWN')
                        {
                            steps {
                                echo "Testing the Project.........."
                            }
                        }
            }
}