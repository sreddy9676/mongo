pipeline{
    agent any 
    stages{
        stage('scm checkout'){
            steps{
                git url:'https://github.com/sreddy9676/mongodb-realtime'
            }
        }
        stage('dev deploy'){
            steps{
                sh "ansible-playbook -i dev.inventory mongodb.yml"
            }
        }
    }
}