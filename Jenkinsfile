pipeline
{
    agent any
    
    stages
    {
        stage ('compile sdsdsz')
        
        {
            steps
            {
                sh 'mvn -f mavewebappdemo/pom.xml install'
            }
        }
        stage ('deploy and once more msjd ')
        
        {
            steps
            {
                sh 'cp -R /root/.jenkins/workspace/pipeline1/mavewebappdemo/target/* /opt/apache-tomcat-8.5.3/webapps'
            }
        }
    }
}
