pipeline{
	agent any 
	stages{
		stage('1-clonecode'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'GitHub-Credentials', url: 'https://github.com/EtechDevOpsProjects/jenkins-github-vscode.git']])
			}
		}
		stage('2-artifactbuild'){
			steps{
				sh 'df -h'    
			}
		}
		stage('3-unittest'){
			steps{
				sh 'lscpu'
			}
		}
	}	
}