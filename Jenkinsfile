def workspace;
node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '7d651da5-ed85-4e60-a6c8-93ac0fe39799', url: 'git@github.com:rbhamra/JenkinsPipeline.git']]])
        workspace =pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
    }
    stage('Build')
    {
        echo "Build the code"
    }
    stage('Unit Testing')
    {
        echo "Unit Testing"
    }
    stage ('Delivery')
    {
        echo "Devliver the Code"
    }
    
}
