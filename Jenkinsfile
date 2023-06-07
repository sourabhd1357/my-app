node {
     stage('SCM Checkout'){
     git 'https://github.com/sourabhd1357/my-app.git'
     }
     stage('Compile package'){
          def mvnhome=tool name: 'myapp_maven', type: 'maven'
          sh "${mvnhome}/bin/mvn package"
     }
}
