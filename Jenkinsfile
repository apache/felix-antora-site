pipeline {
    agent {
        label 'git-websites'
    }

    stages {
        stage('trigger-site-build') {
//             when {
//                 branch 'main'
//                 changeset '**/*'
//             }

            steps {
                triggerRemoteJob remotePathMissing: [$class: 'StopAsFailure'], remotePathUrl: 'jenkins://712657a46c181b3ff60d2c029abcf8b7/Felix/website-build'
            }
        }
    }
}