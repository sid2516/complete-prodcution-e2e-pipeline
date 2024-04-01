# Sample application for e2e DevOps Pipeline
## This is a sample application to demonstrate an end to end DevOps Pipeline

Doc link :- https://docs.dman.cloud/tutorial-documentation/install-sonarqube/#update-sonarqube-properties-with-db-credentials

1.  install java ( url :- https://askubuntu.com/questions/1375383/how-to-properly-install-temurin-jdk-with-update-alternatives )

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
6.  Now configure quality gate in jenkins with web hook  ( name : abc ) ( url : http://jenkins-ip-address :8080/sonarqube-webhook/ )
7.  
