pipeline{
	agent any
	stages{
		stage ( 'Download Prometheus'){
			step{
				sh 'rm -f /tmp/prometheus.tar.gz'
				sh 'wget https://github.com/prometheus/prometheus/releases/download/v2.49.1/prometheus-2.49.1.linux-amd64.tar.gz'			
			
			}		
		}
		
		stage ( 'Archive Prometheus') {
			step{
				sh 'tar -xzf /tmp/prometheus.tar.gz -C /tmp/'
			
			}
		}	
		stage( 'Success'){
			step{
				sh 'echo "Prometheus downloaded successfully"
			}
		}
	}
}
