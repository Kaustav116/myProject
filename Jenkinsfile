pipeline{
agent { label 'Windows'}
tools{
maven 'Maven3'
}
stages{
stage('Checkout'){
steps{
git 'https://github.com/Kaustav116/myProject.git'
}
}
stage('Build'){
steps{
bat 'mvn clean compile'
}
}
stage('Test'){
steps{
bat 'mvn test'
}
}
stage('Package'){
steps{
bat 'mvn package'
}
}
}
}