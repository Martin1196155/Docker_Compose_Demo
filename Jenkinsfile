pipeline{
    tools{
        jdk 'myjava'
        maven 'mymaven'
    }
    
    agent none
    stages{
             stage('Checkout'){
                 agent any
                 steps{
                    git 'https://github.com/Martin1196155/Docker_Compose_Demo.git'
                 }
            }
            stage('Maven_Package'){
                 agent any
                 steps{
                    sh 'mvn -f Java-app/pom.xml package'
                }
            }
    }
}
