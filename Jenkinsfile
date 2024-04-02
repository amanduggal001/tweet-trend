pipeline {
    agent {
        node {
            label "maven"
        }
    }
    
    environment {
        PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
    }
    
    stages {
        stage('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/amanduggal001/tweet-trend.git'  //You can create syntax by selecting the Pipeline syntax option in Jenkins Job.
            }
        }
        stage("Build") {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}
