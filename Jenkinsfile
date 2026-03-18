pipeline {
    agent any
    stages {
        stage ("one") {
            steps {
                git branch: '2026Q1', url: 'https://github.com/127rutu/repo1.git'
                sh "rm -rf /var/www/html/*"
                sh "cp -r index.html /var/www/html"
                
            }
        }
stage ("two") {
            steps {
                git branch: '2026Q2', url: 'https://github.com/127rutu/repo2.git'
                sh "rm -rf /var/www/html/*"
                sh "cp -r index.html /var/www/html"
                
            }
        }
stage ("three") {
            steps {
                git branch: '2026Q3', url: 'https://github.com/127rutu/repo3.git'
                sh "rm -rf /var/www/html/*"
                sh "cp -r index.html /var/www/html"
                
            }
        }

    }
}
