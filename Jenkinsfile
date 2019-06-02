pipeline {
    agent any
    stages {
	
	stage('Git-Checkout') {
        steps {
                echo "Checking out from Git Repo";
                git 'https://github.com/ashkumarverma/jenkins-pipeline.git'
                }
        }

	
        stage('Build') {
            steps {
                echo "Build";
            }
        }

        stage('Unit-Test') {
            steps {
                echo "Unit-Test";
            }
        }

        stage('Quality-Gate') {
            steps {
                echo "Quality-Gate";
            }
        }
    }

    post {
        always {
            echo "always";
        }

        success {
            echo "success";
        }

        failure {
            echo "failure";
        }

        ustable {
            echo "ustable";
        }

        changed {
            echo "changed changed";
            echo "changed";
        }
    }
}