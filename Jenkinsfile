// Powered by Infostretch 

timestamps {

node () {

	stage ('mikofreestyle - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/MachineDragon/jenkinstestpython']]]) 
	}
	stage ('mikofreestyle - Build') {
powershell "python -m unittest discover -s ./src/test/ -p '*_test.py'"
	}
}
}
