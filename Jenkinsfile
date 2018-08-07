pipeline{
agent any
stages{
stage('compile stage'){
	steps{
			withMaven(maven: 'maven_3.5.4'){
			sh 'mvn clean compile'
			}
		}
	}
stage ('two'){
	steps{
			withMaven(maven: 'maven_3.5.4'){
			sh('mvn test')
			}
		}
	}	
stage ('three'){
steps{
echo 'hello all'
}
}

}



}

