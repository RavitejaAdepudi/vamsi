pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                
                    sh 'mavewebappdemo/pom.xml clean install'
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mavewebappdemo/pom.xml  test'
                
            }
        }
        stage('Deploy to Tomcat'){
        steps {
        sh 'cp -r /root/.jenkins/workspace/pipe/target/* /opt/apache-tomcat-8.5.3/webapps/'
        }
        }


        
    }
}
