node {
    def app
     stage('Clone-checkout'){
        checkout scm
     }
     stage('Build image'){
        app = docker.build("dev-python/httpd")
     }
     stage ('Test'){
        withDockerContainer("dev-python/httpd"){ 
            sh "echo 'bonjour ici python'" 
            }
            }
}
