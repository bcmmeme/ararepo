
node {
  properties([parameters([choice(choices: ['start', 'stop'], description: '', name: 'run')])])
  
 stage('run') {
  if ( run == 'start' ) {
      sh '''
       sudo /home1/irteam/tomcat/bin/startup.sh
      '''
  } else if ( run == 'stop' ) {
     sh '''
      sudo /home1/irteam/tomcat/bin/shutdown.sh
      '''
  }
 }
} 
