pipeline{
agent any
stages 
{
stage('docker-compose UP') 
{
steps{
              script {
                  def data = readFile(file: 'docker-compose.yml')
                  println(data)
              }
echo "Before"
echo cd
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
}
}