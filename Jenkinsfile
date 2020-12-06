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
                                bat ('docker-compose -f docker-compose.yml up -d')
                            }
                        }
                stage('Executing Tests')
                        {
                            steps {
                                catchError(buildResult: 'FAILURE', stageResult: 'FAILURE') {
                                    bat ('mvn test')
                                }
                            }
                        }
                stage('docker-compose DOWN')
                        {
                            steps {
                                    bat ('docker stop chrome firefox hub')
                                    bat ('docker rm chrome firefox hub')
                                }
                            }
            }
             post {
                    always {
                        echo 'Done !'
                    }
                }
}