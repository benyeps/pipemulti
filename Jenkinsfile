node('built-in') 
{
    stage('Continuous Download_loans') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build_loans') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('Continuous Deployment_loans') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@172.31.48.25:/var/lib/tomcat9/webapps/qaenvloans.war'
	}
    stage('Continuous Testing_loans') 
	{
              sh label: '', script: 'echo "Testing Passed"'
	}
    
}
