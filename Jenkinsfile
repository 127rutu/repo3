pipeline {
    agent none  // allows specifying different agents per stage

    stages {

        stage("one") {   
            agent { label 'built-in' }
            steps {
                git branch: '2026Q1', url: 'https://github.com/127rutu/repo1.git'
                sh "cp -r index.html /var/www/html"
            }
        }

        stage("two") {  
            agent { label 'slave-1' }
            steps {
                git branch: '2026Q2', url: 'https://github.com/127rutu/repo2.git'
                sh "cp -r index.html /var/www/html"
            }
        }

        stage("three") { 
            agent { label 'slave-2' }
            steps {
                git branch: '2026Q3', url: 'https://github.com/127rutu/repo3.git'
                sh "cp -r index.html /var/www/html"
            }
        }

    }
}
