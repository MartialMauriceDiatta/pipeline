pipeline:
  agent:
    any
  stages:
    - stage: Checkout
      steps:
        - checkout: git@github.com/FallouGAYE/pipeline.git
    - stage: Build
      steps:
        - script:
            - mvn clean install
    - stage: Test
      steps:
        - script:
            - javac -cp .:/path/to/your/junit.jar MainTest.java
            - java -cp .:/path/to/your/junit.jar:/path/to/your/hamcrest.jar org.junit.runner.JUnitCore MainTest
    - stage: Deploy
      steps:
        - script:
            - echo "Déploiement sur le serveur de production en cours"


