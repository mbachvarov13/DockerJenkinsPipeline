pipeline{
agent any
stages
{
stage('docker-compose UP')
{
steps{
echo "Before"
sh "docker-compose -f docker-compose.yml up"
script {
                  def data = readFile(file: 'docker-compose.yml')
                  println(data)
              }
echo "After"
}
}
stage('Executing Tests')
{
steps{
echo "Testing the Project.........."
}
}
stage('docker-compose DOWN')
{
steps{
echo "Testing the Project.........."
}
}
<<<<<<< HEAD
=======
}
=======
pipeline {
    agent any
    stages
            {
                stage('docker-compose UP')
                        {
                            steps {
                                sh ("pwd")
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
>>>>>>> 26478fd2c01ac45d43a373d629f71e92c0f6d678
>>>>>>> 7823a3df49dbb268b43e714062365d53c93a70dd
}