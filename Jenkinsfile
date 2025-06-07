pipeline { 
    agent any 

    tools { 
        maven 'Maven' // Ensure this matches the Maven tool name configured in Jenkins
    } 

    stages { 
        stage('Checkout') {  
            steps { 
                git branch: 'master', url: 'https://github.com/RakeshAM10/Hello.git'  
            } 
        } 

        stage('Build') {  
            steps { 
                bat 'mvn clean package'  
            } 
        } 

        stage('Test') {  
            steps { 
                bat 'mvn test'  
            } 
        } 

       stage('Run Application') {  
           steps { 
              bat 'java -jar target\\Hello2-0.0.1-SNAPSHOT.jar'

              }
         }
     } 
}
Kind: Secret text
Secret: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
ID: github-token

Pipeline stage view plugin 
Maven integration plugin 
Gradle integration plugin 
Github integration plugin

For Freestyle project type:
Under Build, add a build step Invoke top-level Maven targets

Enter goals like clean install

Configure SCM as above
