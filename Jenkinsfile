node{
    stage('SCM Checkout'){
        
        git 'https://github.com/nacer-noubir/my_app'  
    }
    stage('Compile-Package'){
        def mvnHome = tool 'M3'
        sh "${mvnHome}/bin/mvn package"
    }
}
