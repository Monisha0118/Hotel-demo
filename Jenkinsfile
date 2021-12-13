node{
  
  stage('code build'){
    git 'https://github.com/Monisha0118/Hotel-demo.git'
  }
  stage('build') {
    def mvnHome = tool name: 'maven3', type: 'maven'
    sh "${mvnHome}/mvn clean install"
  }
  stage('deploy to tomcat') {
    sh "cp -r /var/lib/jenkins/workspace/Hotel-Webapplication/target/hotel.war /opt/apache-tomcat-9.0.56/webapps/"
   }
}
