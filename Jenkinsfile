pipeline{
  agent any
  tools {maven "mavenv4"}
  stages{

    stage("checkout"){
      steps{
        git branch: "main" , url: "https://github.com/udvale/SpringRESTful.git"
      }
    }

    stage("build"){
      steps{
        sh "mvn compile"
      }
    }

    stage("test"){
      steps{
        sh "mvn test"
      }
    }
  }
}
