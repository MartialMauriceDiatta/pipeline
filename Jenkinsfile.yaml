pipeline:
  agent: any
  stages:
    - name: Checkout
      steps:
        - checkout: scm
    - name: Build
      steps:
        - bat: 'javac HelloWorld.java'
    - name: Test
      steps:
        - bat: 'java HelloWorld'
    - name: Deploy
      steps:
        - echo: "Déploiement sur le serveur de production en cours"
