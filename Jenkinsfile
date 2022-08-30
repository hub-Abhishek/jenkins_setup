def gv

pipeline {
    agent any
    parameters {
        choice(name: 'VERSION', choices: ['1.1.0', '1.2.0', '1.3.0'], description: '')
        booleanParam(name: 'executeTests', defaultValue: true, description: '')
    }
    stages {
        stage("init") {
            steps {
                echo 'stage 1'
            }
        }
        stage("build") {
            steps {
                echo 'stage 2'
                python3 hello_world.py
            }
        }
        stage("deploy") {
            steps {
                echo 'stage 3'
            }
        }
    }
}