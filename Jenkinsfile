node {
    stage 'Building image'
    git 'https://github.com/satishthamarana/docker-springboot-jenkins-example-master.git' // checks out Dockerfile
    def myEnv = docker.build 'cqueiroz:snapshot'
    myEnv.inside {
        sh 'mvn clean package'
    }
}
