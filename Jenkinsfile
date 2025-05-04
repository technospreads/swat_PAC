pipeline {
    agent any

    stages {
        stage('stage1') {
            steps {
                script {
                    // myplayground
                    var1= 20
					string="This is Jenkins-PAC"
                    echo 'Hello, welcome to Jenkins PAC'
					println "Here is your userdefined variables ${var1},${string}"
					println "Here is your global/predefined variables ${currentBuild.result}"
					println "Here is your global/predefined variables ${currentBuild.id}"
					println "Here is your global/predefined environment variables ${env.JOB_NAME}"
                    
                }
            }
        }
    }
}
