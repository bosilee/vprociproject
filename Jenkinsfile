pipeline{
    
    agent any
    tools {
        maven "MAVEN3"
        jdk "OracleJDK"
        
    }

    environment {
        SNAP_REPO = 'bosiprofile-snapshot'
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'Kushenla24?'
        RELEASE_REPO = 'bosiprofile-release'
        CENTRAL_REPO = 'bosipro-maven-central'
        NEXUSIP = '172.31.55.246'
        NEXUSPORT = '8081'
        NEXUS_GRP_REPO = 'bosiprofile-maven-grou-'
        NEXUS_LOGIN = 'nexuslogin'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}