pipeline 
{
agent any
  stages 
  {
    stage('verify branch')
    {
      steps 
      {
        echo "$GIT_BRANCH"
      }
    }
    stage('Build')
    {
      steps
      {
        pwsh(script: 'mvn package')
      }
    }
  }
}
