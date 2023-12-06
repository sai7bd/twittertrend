pipeline{
    agent {
        node {
            label "valaxy"
        }
    }
    environment {
        PATH = "/opt/apache-maven-3.8.8/bin:$PATH"
    }    
    stages {
        stage('build') {
            steps{
                echo "------------ build started ---------"
                sh 'mvn clean deploy -Dmaven.test.skip=true'
                echo "------------ build completed ---------"
        }
    }
}

}

    
  
