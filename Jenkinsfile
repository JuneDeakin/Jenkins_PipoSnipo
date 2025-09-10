pipeline{
    agent any 
    stages{
        stage("Build"){
            steps{
                echo "Building ..."
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
    }
}
            



}
