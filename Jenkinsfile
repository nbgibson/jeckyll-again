pipeline {
    agent any

    environment {
        //DOCKERUSER = credentials('dockerUsername')
        //DOCKERTOKEN = credentials('dockerToken')
    }
    stages {
        stage('Docker Build') {
            steps {
                sh 'echo "hello, world!"'
                /*sh '''
                echo $DOCKERUSER
                cat version
                echo "$DOCKERTOKEN" | docker login -u $DOCKERUSER --password-stdin 
                docker build . --label build_date=$(date +%Y-%m-%d) -t $(echo $DOCKERUSER)/ytdl:$(cat version)
                docker push $(echo $DOCKERUSER)/ytdl:$(cat version)
                docker build . --label build_date=$(date +%Y-%m-%d) -t $(echo $DOCKERUSER)/ytdl:latest
                docker push $(echo $DOCKERUSER)/ytdl:latest
                '''*/
            }
        }
    }
}