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
                                bat 'docker-compose -f docker-compose.yml up -d'
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
                                bat 'docker stop dockerjenkins_chrome_1 dockerjenkins_firefox_1 dockerjenkins_hub_1'
                                bat 'docker rm dockerjenkins_chrome_1 dockerjenkins_firefox_1 dockerjenkins_hub_1'
                            }
                        }
            }
}