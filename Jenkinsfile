pipeline {
    agent { label 'built-in' }

    stages {
        stage("Deploy Repo1") {
            steps {
                dir('repo1') {
                    git branch: '2026Q1', url: 'https://github.com/127rutu/repo1.git'
                    sh 'cp index.html /var/www/html/index1.html'
                }
            }
        }

        stage("Deploy Repo2") {
            steps {
                dir('repo2') {
                    git branch: '2026Q2', url: 'https://github.com/127rutu/repo2.git'
                    sh 'cp index.html /var/www/html/index2.html'
                }
            }
        }

        stage("Deploy Repo3") {
            steps {
                dir('repo3') {
                    git branch: '2026Q3', url: 'https://github.com/127rutu/repo3.git'
                    sh 'cp index.html /var/www/html/index3.html'
                }
            }
        }
    }
}
