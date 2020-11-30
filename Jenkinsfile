pipeline{
agent any
stages 
{
stage('docker-compose UP') 
{
steps{
echo "Testing the Project.........."
sh "docker-compose up -d"
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