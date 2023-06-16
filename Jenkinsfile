
pipeline {
  agent any
  parameters {
        string(name: 'PERSON', defaultValue: 'Jenkins', description: 'Who should I say hello to?')
    }
  stages{
    stage('first') {
      steps{
      
        script {runPerson ()}
        //script { echo "${params.PERSON}" }
        


      }
    }
  }
  void runPerson () {
      if (PERSON == 'Jenkins') {
            // publish to the /nr-smbd-snapshots
            echo "It's: Jenkins"
        } else {
            echo "It's not a Jenkins"
        }
  }
}
