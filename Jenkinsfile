pipeline {
    agent {
        label {
            label "slave1"
        customWorkspace "/mnt/git"
        }
        
    }

    stages {
        stage ('Compile Stage') {

            steps {
                
                    sh 'mvn clean compile'
                }
            
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
                }
            
        }


        stage ('Install Stage') {
            steps {
                
                    sh 'mvn install'
                }
            
        }
        
        stage ('Echo Branch') {

            steps {
                
                    echo "This is master branch"
                }
            
        }
    }
}
