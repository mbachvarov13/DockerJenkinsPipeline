pipeline {
    agent any
    stages
            {
                stage('docker-compose UP')
                        {
                            steps {
                                echo "Before"
                                sh "docker-compose build"
                                sh "docker-compose up -d"
                                script {
                                    def data = readFile(file: 'docker-compose.yml')
                                    println(data)
                                }
                                echo "After"
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