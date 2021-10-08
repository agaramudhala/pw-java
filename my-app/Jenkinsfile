#!/usr/bin/env groovy

Jenkinsnode('node'){
docker.image('pro-node-playwright').inside{
    stage('checkout'){
        scmcheckout {}
    }
    stage('Install'){
        sh 'mvn -v'
        sh 'mvn compile exec:java -Dexec.mainClass=com.mycompany.app.Example'
    }
}
}
