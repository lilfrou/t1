pipeline {
    agent any
    stages {
        stage('Example') {
            options {
                timeout(time: 1, unit: 'HOURS') 
            }
            when { 
  allOf { 
    expression { env.GITHUB_PR_STATE == "CLOSE" }
    expression { env.GITHUB_PR_TARGET_BRANCH == "main" }
  } 
}

            steps {
                echo 'Hello World'
                echo 'Hello World'
                echo 'Hello World'
            }
        }
    }
}
