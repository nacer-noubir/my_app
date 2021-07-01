node{
    stage('SCM Checkout'){
        
        git 'https://github.com/nacer-noubir/my_app'  
    }
    stage('Compile-Package'){
        def mvnHome = tool name: 'M3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
}
