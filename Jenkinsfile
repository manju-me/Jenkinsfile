pipeline{
    agent any
    environment{
        PATH ="/opt/maven/bin:$PATH"
        }
    stages{
        stage('Git clone'){
            steps{
                git url: 'https://github.com/SaiDevOpsFaculty/war-web-project.git', branch: 'master'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn clean install'
            }
        }    
    }
   }
