# Sample application for e2e DevOps Pipeline
## This is a sample application to demonstrate an end to end DevOps Pipeline

Doc link :- https://docs.dman.cloud/tutorial-documentation/install-sonarqube/#update-sonarqube-properties-with-db-credentials

1.  install java 
      wget -O - https://packages.adoptium.net/artifactory/api/gpg/key/public | sudo apt-key add -
      echo "deb https://packages.adoptium.net/artifactory/deb $(awk -F= '/^VERSION_CODENAME/{print$2}' /etc/os-release) main" | sudo tee /etc/apt/sources.list.d/adoptium.list
    sudo apt update
    sudo apt install temurin-17-jdk

2.  install jenkins from doc
3.  install sonar from doc on other server
4.  install docker on both server
5.  install plugins in jenkins
        -   adoptium   ( this is use for java tool setup in jenkins )
        -   maven
        -   docker
        -   pipeline plugins
        -   sonarscanner
        -   junit
        -   slack
        -   sonarscanner
        -   AWS all
6.  Now configure quality gate in jenkins with web hook  ( name : abc ) ( url : http://sonarqube-ip-address/sonarqube-webhook/ )
7.  
