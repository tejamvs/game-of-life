node{
   
   stage('scm')'{'
   git 'https://github.com/tejamvs/game-of-life'
}
stage ('Build & package') {
    sh 'mvn package'
}
stage ( 'results')'{
      archive 'gameoflife-web/target/gameoflife.war'
      junit 'gameoflife-web/target/surefire-reports/*xml'
}
   }