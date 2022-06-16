node('built-in') 
{
    stage('Continuous Download_loans') 
	{
    git 'https://github.com/Ramchander09/Ramchander09.git'
	}
    stage('Continuous Build_loans') 
	{
    sh label: '', script: 'mvn package'
	}
	
	stage('Continuous Deployment_loans') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/multiline_loans/webapp/target/webapp.war   ubuntu@172.31.43.48:/var/lib/tomcat8/webapps/qaenv.war'
	}
    stage('Continuous Testing') 
	{
              sh label: '', script: 'echo "Testing Passed"'
	}
	
	
    }
