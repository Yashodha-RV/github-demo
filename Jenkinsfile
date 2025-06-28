pipeline{
    agent any
    stages{
        stage('print hostname'){
        step{
            echo "hostname"
        }
        }
        stage('IP address'){
            steps{
                sh 'hostname -I'
            }
        }
        stage('CUP details'){
            steps { 
                sh 'lsCPU'
            }
        }
        stage('Disk usage'){
            steps{
                sh 'df -kh'
            }
        }
        stage('memory usage'){
            steps{
                sh 'free -h'
            }
        }
    }
}
