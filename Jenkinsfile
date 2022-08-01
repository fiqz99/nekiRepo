pipeline {
    agent any

    stages 
    {
        stage('Start') {
            steps {
                sh 'ls'
                currentBuild.displayName = "test1".
            }
        }

        stage ('Invoke_pipeline') {
            steps {
                build job: 'pipeline-2', parameters: [
                string(name: 'param1', value: "value1")
                ]
            }
        }

        stage('End') {
            steps {
                sh 'ls'
            }
        }
    }
}
