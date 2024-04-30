pipeline {
    
	agent any
	
	tools {
        maven "MAVEN3"
        jdk "OracleJDK11"
    }
	
    environment {
        SNAP_REPO = 'vprofile-snapshot'
        NEXUS_USER = 'admin'
        NEXUS_PASS = '0930@Rey'
        RELEASE_REPO = 'vprofile-release'
        CENTRAL_REPO = 'vpro-maven-central'
        NEXUS_GRP_REPO = 'vpro-maven-group'
        NEXUSIP = '172.31.54.165'
        NEXUSPORT = '8081'
        NEXUS_LOGIN = 'nexuslogin'

        
    }
	
    stages{
        
        stage('BUILD'){
            steps {
                sh 'mvn -s settings.xml -DskipTests install'
            }
            
        }
    }

	


}
