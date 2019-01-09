pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                
                    sh 'mvn clean install'
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
                
            }
        }
        stage('Deploy to Tomcat'){
        steps {
        sh 'cp -r /root/.jenkins/workspace/pipe/vamsi/target/* /opt/apache-tomcat-8.5.3/webapps/'
        }
        }


        
    }
}
