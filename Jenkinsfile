pipeline{
agentany
tools{
maven'Maven3'
}
stages{
stage('Checkout') {
steps{
gitbranch: 'main', url: 'https://github.com/<your-username>/maven-test-demo.git'
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