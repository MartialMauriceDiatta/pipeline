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
            - mvn test
    - stage: Deploy
      steps:
        - script:
            - echo "Déploiement sur le serveur de production en cours"

