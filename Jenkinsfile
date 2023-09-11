pipeline {
    agent any
    stages {
        stage('BackEnd') {
            steps {
                sh "rm -rf TicketBookingServiceJunitTesting"
                sh "git clone https://github.com/kishancs2020/TicketBookingServiceJunitTesting.git"
                sh "mvn clean -f TicketBookingServiceJunitTesting"
            }
        }
        stage('FrontEnd') {
           steps {
                sh 'echo "FontEnd is running on port 4200!"'
            }
        }
    }
}

