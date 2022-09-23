node {
    def app
     stage('Clone-checkout'){
        checkout scm
     }
     stage('Build image'){
        app = docker.build("dev-python/apache")
     }
     stage ('Test'){
        withDockerContainer("dev-python/apache"){ 
            sh "echo 'bonjour ici python'" 
            }
            }
}
