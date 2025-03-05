pipeline{
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Ametovali/task3_project.git'
            }
        }

        stage('Build Java Program') {
            steps {
                bat 'javac -d out src/main/java/com/repeat/HelloWorld.java'
            }
        }

        stage('Run Java Program') {
            steps {
                bat 'java -cp out com.repeat.HelloWorld'
            }
        }
    }
}
