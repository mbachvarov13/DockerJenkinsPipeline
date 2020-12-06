pipeline {
    agent any
    stages
            {
                stage('docker-compose UP')
                        {
                            steps {
                                bat 'docker ps -a'
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