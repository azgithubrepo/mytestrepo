pipeline{
agent any
stages{
stage('compile stage'){
	steps{
			withMaven(maven : 'maven_3.5.4'){
			sh 'mvn clean compile'
			}
		}
	}
stage ('test'){
	steps{
			withMaven(maven : 'maven_3.5.4'){
			sh('mvn test package')
			}
		}
	}	
stage ('Deploy into tomcat'){
steps{
sh 'scp  home/ajay/.jenkins/workspace/FirstPipeline/*.war /home/ajay/Downloads/apache-tomcat-7.0.90/webapps/'
}
}

}



}

