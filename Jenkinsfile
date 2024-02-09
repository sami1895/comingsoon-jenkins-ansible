pipeline {
    agent any

    environment {
		DOCKERHUB_CREDENTIALS=credentials('dockerhub')
	}
    stages {
        stage('Build & push Dockerfile') {
            steps {
                sh """
		ansible-playbook ansible-playbook.yml
                """
            }
        }
    } 
}
