node('built-in') 
{
    stage('Continuous Download_Master') 
	{
    git 'https://github.com/Ramchander09/Ramchander09.git'
	}
    stage('Continuous Build_Master') 
	{
    sh label: '', script: 'mvn package'
	}
    
}
