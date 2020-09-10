
node {
  properties([parameters([choice(choices: ['start', 'stop'], description: '', name: 'run')])])
  
 stage('run') {
  if ( param.run == 'start' ) {
      sh '''
       sudo /home1/irteam/tomcat/bin/startup.sh
      '''
  } else if ( param.run == 'stop' ) {
     sh '''
      sudo /home1/irteam/tomcat/bin/shutdown.sh
      '''
  }
 }
} 
