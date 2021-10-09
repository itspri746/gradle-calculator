pipeline
{
agent any
stages
{
  stage ('code scm checkout')
  { steps { git branch: 'master', url: 'https://github.com/itspri746/gradle-calculator'  } }

  stage ('code build')
  { steps { sh './gradlew clean build'
            sh './gradlew jar'}}

  stage ('code test')
  { steps { sh './gradlew test'}}

}
}
