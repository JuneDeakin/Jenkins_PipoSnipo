pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "=============================="
                echo "Stage 1: Build"
                echo "Tool: Maven"
                echo "Action: Compile and package the code."
                echo "=============================="
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo "=============================="
                echo "Stage 2: Unit and Integration Tests"
                echo "Tools: JUnit (unit testing), TestNG (integration testing)"
                echo "Action: Validate code functionality and component interactions."
                echo "=============================="
            }
        }

        stage('Code Analysis') {
            steps {
                echo "=============================="
                echo "Stage 3: Code Analysis"
                echo "Tool: SonarQube"
                echo "Action: Perform static code analysis and ensure industry standards are met."
                echo "=============================="
            }
        }

        stage('Security Scan') {
            steps {
                echo "=============================="
                echo "Stage 4: Security Scan"
                echo "Tool: OWASP Dependency-Check"
                echo "Action: Identify vulnerabilities in code dependencies."
                echo "=============================="
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "=============================="
                echo "Stage 5: Deploy to Staging"
                echo "Environment: AWS EC2 (Staging)"
                echo "Action: Deploy application to a staging server."
                echo "=============================="
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "=============================="
                echo "Stage 6: Integration Tests on Staging"
                echo "Tool: Selenium"
                echo "Action: Verify application behavior in a production-like environment."
                echo "=============================="
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "=============================="
                echo "Stage 7: Deploy to Production"
                echo "Environment: AWS EC2 (Production)"
                echo "Action: Deploy application to the production server."
                echo "=============================="
            }
        }
    }

    post {
        always {
            echo "==========================================="
            echo "Pipeline completed – All stages executed."
            echo "==========================================="
        }
    }
}
