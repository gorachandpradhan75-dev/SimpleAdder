node {
    def mvnHome = tool 'Maven-3.9.16'

    stage('Checkout') {
        git branch: 'main',
            url: 'https://github.com/gorachandpradhan75-dev/SimpleAdder.git'
    }

    stage('Validate') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" validate"
    }

    stage('Compile') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" compile"
    }

    stage('Test') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" test"
    }

    stage('Package') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" package"
    }

    stage('Verify') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" verify"
    }

    stage('Install') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" install"
    }

    stage('Site') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" site"
    }

    stage('Clean') {
        bat "\"${mvnHome}\\bin\\mvn.cmd\" clean"
    }
}