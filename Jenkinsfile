pipeline {
    agent any
	environment {
  SUBJECT = "JENKINS_PAC"
}
parameters {
  choice choices: ['dev', 'sit', 'qa', 'pre-prod', 'prod'], name: 'environment'
}
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
					println "Here is your defined environment variables ${env.SUBJECT}"
					println " Here is your defined parameterised variable and you have choosen envirnment is : ${params.environment}"
                    
                }
            }
        }
    }
}
