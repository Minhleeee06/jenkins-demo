pipeline {
    agent any

    stages {
        stage('Stage 1: Build') {
            steps {
                echo 'Stage 1 Build'
                echo 'Tasks: Compile and package the source code into a deployable artifact.'
                echo 'Tool: Maven'
            }
        }
        stage('Stage 2: Unit and Integration Tests') {
            steps {
                echo 'Stage 2 Test'
                echo 'Task: Run unit tests and integration tests.'
                echo 'Tool: JUnit and Selenium'
            }
        }
        stage('Stage 3: Code Analysis') {
            steps {
                echo 'Stage 3 code analysis'
                echo 'Task: Analyse source code.'
                echo 'Tool: Checkstyle'
            }
        }
        stage('Stage 4: Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Perform a security scan.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }
        stage('Stage 5: Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploy to a staging server.'
                echo 'Tool: AWS CLI'
            }
        }
        stage('Stage 6: Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Execute integration tests against staging.'
                echo 'Tool: Postman / Newman'
            }
        }
        stage('Stage 7: Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploy to the live production server.'
                echo 'Tool: AWS CLI'
            }
        }
    }
    post {
        success {
            echo 'Pipeline completed successfully across all 7 stages.'
        }
        failure {
            echo 'Pipeline encountered an error.'
        }
    }
}