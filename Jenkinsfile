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
                                bat 'docker-compose -f docker-compose up -d'
                            }
                        }
                stage('Executing Tests')
                        {
                            steps {
                                bat 'mvn test'
                            }
                        }
                stage('docker-compose DOWN')
                        {
                            steps {
                                bat 'docker-compose -f docker-compose down'
                            }
                        }
            }
}