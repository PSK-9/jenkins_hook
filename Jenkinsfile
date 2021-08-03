pipeline {
    agent any
    stages {
//        stage('Git-Clone') {
    //        steps{
      //          git url:'https://github.com/kliakos/sparkjava-war-example.git'
           // }
       // }
        stage('Build') {
            steps {
                sh 'mvn clean package'

            }
        }
        stage('Deploy') {
            steps{
                  sh 'cp -f target/sparkjava-hello-world-1.0.war /usr/java/apache-tomcat-8.5.69/webapps'
        }    
        }
}
}
