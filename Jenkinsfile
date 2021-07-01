node{
    stage('SCM Checkout'){
        git 'https://github.com/nacer-noubir/my_app'  
    }
    stage('Compile-Package'){
        sh 'mvn package'      
    }
}
