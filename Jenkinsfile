pipeline
{
    agent any
    
    stages
    {
        stage ('compile')
        
        {
            steps
            {
                sh 'mvn -f mavewebappdemo/pom.xml install'
            }
        }
        stage ('compile')
        
        {
            steps
            {
                sh 'cp -R /root/.jenkins/workspace/pipeline1/target/* /opt/apache-tomcat-8.5.3/webapps'
            }
        }
    }
}
