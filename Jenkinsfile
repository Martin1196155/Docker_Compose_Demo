pipeline{
    tools{
        jdk 'myjava'
        maven 'mymaven'
    }
    
    agent none
    stages{
            stage('Compile'){
                agent any
                steps{
                    sh 'mvn compile'
                }
            }
}
