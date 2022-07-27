pipeline {
    agent any
    parameters
    {
	booleanParam(name: "sonarScan",default: "true", description: "To run Sonar Scan on Project")
    }
    stages
    {
        stage("scan") {
            steps {
                echo 'Scanning the directory'
            }
        }
        stage("build") {
            steps {
                echo 'Building the directory'
            }
        }
        stage("test") {
            steps {
                echo 'testing the directory'
            }
        }
    }
}


