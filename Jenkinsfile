node{
    stage('SCM Checkout'){
        
        git 'https://github.com/nacer-noubir/my_app'  
    }
    stage('Compile-Package'){
        def mvnHome = tool name: 'M3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
    stage('Email Notification'){
        mail bcc: '', body: '''Hi!
        This is a jenkins email notif

        Robi''', cc: '', from: '', replyTo: '', subject: 'Jenkins JO', to: 'nacer.noubir@gmail.com'
    }
}
