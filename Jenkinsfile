pipeline{
    
    agent {label 'linagent'}
    
    stages{
        stage('build'){
        steps{
            sh 'echo hello'
           // sh 'git clone https://github.com/sneha0302/java-reachability-playground.git'
     
	sh 'docker pull gesellix/trufflehog'
	sh 'docker run gesellix/trufflehog --json --regex https://github.com/sneha0302/java-reachability-playground.git > result'
	sh 'cat result'
	        }
            
            
        }
        
        
    }
    
    
}
