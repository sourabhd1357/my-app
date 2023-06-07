node {
     stage('SCM Checkout'){
     git 'https://github.com/sourabhd1357/my-app.git'
     }
     stage('Compile package'){
          def mvnhome=tool name: 'myapp_maven', type: 'maven'
          sh "${mvnhome}/bin/mvn package"
     }
     stage('Email Notification'){
mail bcc: '', body: '''This is the jenk email alerts
from the system
Bye!!!!!!!!!!!!!''', cc: '', from: '', replyTo: '', subject: 'Jenkins my-app job', to: 'sourabhd1357@gmail.com'     }
}
