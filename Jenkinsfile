pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '/var/jenkins_home/apache-maven-3.8.4/bin/mvn clean verify sonar:sonar \
  -Dsonar.projectKey=FirstProject \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.login=246520bf58bf82ab8d51e55c5e3e1b69b8ad4a86'
               }
        }
    }
}
