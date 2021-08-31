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
sh 'mvn clean compile'
}
}
stage('Test'){
steps{
sh 'mvn test'
}
}
stage('Package'){
steps{
sh 'mvn package'
}
}
}
}