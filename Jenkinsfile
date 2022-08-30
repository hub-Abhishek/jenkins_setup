pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            steps {
                echo 'Compile Stage Complete'
            }
        }

        stage   ('Testing Stage') {
            steps {
                python3 hello_world.py
                echo 'Testing Stage Complete'
            }
        }

        stage ('Build Stage Complete') {
            steps {
                echo 'Build Stage Complete'
            }
        }

    }
}