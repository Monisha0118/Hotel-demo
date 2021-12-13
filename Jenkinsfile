node{
  
  stage('code build'){
    git 'https://github.com/Monisha0118/Hotel-demo.git'
  }
  stage('build') {
    def mvnHome = tool name: 'maven3', type: 'maven'
    sh "${mvnHome}/bin/mvn clean install"
  }
}
