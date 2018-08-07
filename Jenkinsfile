node {
    stage 'Building image'
    git 'https://github.com/satheeshchepuri/docker-springboot-jenkins-example-master' // checks out Dockerfile
    def myEnv = docker.build 'cqueiroz:snapshot'
    myEnv.inside {
        sh 'mvn clean package'
    }
}
