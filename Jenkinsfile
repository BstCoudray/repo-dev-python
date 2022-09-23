node {
    def app
     stage('Clone-checkout'){
        checkout scm
     }
     stage('Build image'){
        app = docker.build("devpython/httpd")
     }
     stage ('Test'){
        withDockerContainer("devpython/httpd"){ 
            sh "echo 'bonjour ici python'" 
            }
            }
}
