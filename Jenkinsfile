pipeline 
{
    agent any

    stages
     {
        stage('hello') 
        {
            steps 
            {
              sh 'echo Hello world chanchu1'
              
            }
         }
        stage('build') 
        {
            steps 
            {
              sh 'echo build app'
              
            }
         }
         stage('test') 
        {
            steps 
            {
              sh 'echo test app'
              
            }
         } 
         stage('deploy') 
        {
            steps 
            {
              sh 'echo deploy app'
              
            }
         }
      }
   post
   {
     failure
     {
      emailext body: 'hello', subject: 'this is regards with file', to: 'chanchalaa44@gmail.com'
     }
   }  
}
