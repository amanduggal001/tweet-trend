pipeline {
    agent {
        node {
            label "maven"
        }
    }

    stages {
        stage('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/amanduggal001/tweet-trend.git'
            }
        }
    }
}
