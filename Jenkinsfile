pipeline{
agentany
tools{
maven'Maven3'
}
stages{
stage('Checkout') {
steps{
gitbranch: 'main', url: 'https://github.com/VR-Sindhujha/maven-2.git'
}
}
stage('Compile') {
steps{
bat 'mvncleancompile'
}
}
stage('Test'){
steps{
bat 'mvntest'
}
}
}
}