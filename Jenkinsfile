pipeline {
    agent any
	tools {
    maven "MAVEN_HOME"
}
    stages
            {
                stage('docker-compose UP')
                        {
                            steps {
                                bat 'mvn'
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