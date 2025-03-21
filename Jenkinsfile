pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
    pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application to Tomcat...'
                sh '''
                WAR_FILE=target/NumberGuessGame.war
                TOMCAT_USER=admin
                TOMCAT_PASS=admin_password
                TOMCAT_HOST=your_server_ip_or_domain
                TOMCAT_PORT=8080
                
                curl -v -u $TOMCAT_USER:$TOMCAT_PASS \
                -T $WAR_FILE "http://$TOMCAT_HOST:$TOMCAT_PORT/manager/text/deploy?path=/NumberGuessGame&update=true"
                '''
            }
        }
    }
}

