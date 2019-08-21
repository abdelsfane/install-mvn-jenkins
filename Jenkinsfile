node {
  checkout scm
  
  stage("Update") {
      sh '''
      echo "Updating...!"
      sudo apt-get update -y
    '''
  }
  stage("Install Maven") {
      sh '''
      echo "Installing Maven!"
        sudo apt install maven -y
        '''
  }
  stage("Version") {
      sh '''
      echo "What is the version!"
        mvn -version
        '''
  }
}
