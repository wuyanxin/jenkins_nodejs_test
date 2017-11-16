//pipeline {
  //  agent any
    //stages {
        //stage('build') {
            //steps {
          //      bat 'npm --version'
        //    }
      //  }
    //}
//}


// <1> -  allocates an executor and workspace in the Jenkins environment.
node { 

    // <2> -  describes distinct parts of the Pipeline for better visualization of progress/status.
    stage('Checkout') { 
        
         //bat 'git pull origin master'

         //bat 'npm install'

        // checkout code from source control - 
        // scm is a special variable which instructs the checkout step to clone the specific 
        // revision which triggered this Pipeline run

        checkout scm

        bat 'npm install'

        echo 'npm version:'
        bat 'npm -v'

        echo 'jasmine-node version:'
        bat 'jasmine-node --version'

        bat 'npm run test'

        echo 'Builded!'

    }
    stage('Test') {
        //bat 'npm run --silent lint > TEST_RESULTS/eslint.xml'
    }
}
