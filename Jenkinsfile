node
{
    stage('checkout scm'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/shweta1021/sample-java-programs.git']]])   
        }
    stage ('shell script'){
        sh label: '', script: 'mvn install'
    }
    stage('build'){
        echo 'build is successful'
    }
    stage ('deploy'){
        echo 'done with deployment'
    }
    stage('deliver'){
        echo 'delivered'
    }
    
    
   
}
