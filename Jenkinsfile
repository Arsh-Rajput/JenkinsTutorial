pipeline {
    agent any
    parameters
    {
	booleanParam(name: "sonarScan",defaultValue: "true", description: "To run Sonar Scan on Project")
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
        stage("sonarScan")
        {
            when{
                expression
                {
                    params.sonarScan
                }
            }
        }
        stage("test") {
            steps {
                echo 'testing the directory'
            }
        }
    }
}


