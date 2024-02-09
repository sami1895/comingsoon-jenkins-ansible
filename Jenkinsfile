pipeline {
    agent any

    environment {
		DOCKERHUB_CREDENTIALS=credentials('dockerhub')
	}
    stages {
        stage('Build & push Dockerfile') {
            steps {
                sh """
		cd comingsoon-jenkins-ansible
		ansible-playbook ansible-playbook.yml
                """
            }
        }
    } 
}
