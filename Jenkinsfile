pipeline{
	agent { label 'java'}
	stages{
		stage ('Dowload Prometheus'){
			steps{
				sh 'rm -f /tmp/prometheus.tar.gz'
				sh 'wget https://github.com/prometheus/prometheus/releases/download/v2.49.1/prometheus-2.49.1.linux-amd64.tar.gz'			
			
			}		
		}
		
		stage ('Archive Prometheus') {
			steps{
				sh 'tar -xzf /tmp/prometheus.tar.gz -C /tmp/'
			
			}
		}	
		stage('Success'){
			steps{
				sh 'echo "Prometheus downloaded successfully'
			}
		}
	}
}

