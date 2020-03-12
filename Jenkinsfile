// define a global variable
def workspace;

node {
    stage('Checkout'){
        checkout([$class: 'GitSCM', 
        branches: [[name: '*/master']], 
        doGenerateSubmoduleConfigurations: false, 
        extensions: [],
        submoduleCfg: [],
        userRemoteConfigs: 
        [[credentialsId: '1e064473-4d7d-46e5-bb88-5f893a5e05b2', 
        url: 'https://github.com/mimal/PipelineAsACode.git']]])
     
        workspace=pwd()
    }
    stage('Static Code Analysis'){
        echo "Static code Analysis"
    }
    stage('Build'){
        echo "Build the code"
    }
    stage('Unit Testing'){
        echo "Unit Testing"
    }
    stage('Delivery'){
        echo '"Delivery the Code'
    }
}
