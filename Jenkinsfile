node {
    stage('SCM checkout') {
        stpes {
            sh "rm -rf test-pipeline && git clone https://github.com/Pensu/test-pipeline"
        }
    }
    stage('Docker build') {
        steps {
            sh "cd test-pipeline && docker build -t test:${BUILD_NUMBER} ."
        }
    }
}
