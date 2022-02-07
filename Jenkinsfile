node {
 stage('SCM') {
     echo 'Gathering code from version control'
 }
 stage('Build') {
  try{
  echo 'Building ....'
  sh "dotnet --version" 
  }catch(ex){
      echo 'Something went wrong'
      echo ex.toString();
      currentBuild.result = 'FAILURE'
  }
  finally{
     // cleanup
  }
 
 
 }
 stage('Test') {
  echo 'Testing ....'
  
 }
 stage('Deploy') {
  echo 'Deploying ....'
  
 }

}