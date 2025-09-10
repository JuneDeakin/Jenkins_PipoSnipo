pipeline{
    agent any 
    stages{
        stage("Build"){
            steps{
                echo "Building..."
                echo "Building build.gradle"
                echo "Compiling code..."
                echo "Build complete."
            }
            post{
                success{
                    mail to: "247minijune@gmail.com",
                    subject: "Build Status Email",
                    body: "Build was successful!"
                }
            }
        }
    stage("Test"){
        steps{
            echo "Testing..."
        }
    }
    stage("Deploy"){
        steps{
            echo "Deploying..."
        }
    }
        stage("Comeplete"){
        steps{
            echo "Completed!"
        }
    }
    }
}

