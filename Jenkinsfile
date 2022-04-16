pipeline{
    
    agent {label 'linagent'}
    
    stages{
        stage('build'){
        steps{
            sh 'echo hello'
           // sh 'git clone https://github.com/charankk21/Trufflehog.git'
     
	sh 'docker pull gesellix/trufflehog'
	sh 'docker run gesellix/trufflehog --json --regex https://github.com/charankk21/Trufflehog.git > result'
	sh 'cat result'
	        }
            
            
        }
        
        
    }
    
    
}
