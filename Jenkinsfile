pipeline {
   agent any
   environment{
       BUNPATH="${HOME}/.bun/bin"
   }
   stages {
     stage('Install bun') {
       steps {
         sh 'curl -fsSL https://bun.sh/install | bash -s "bun-v1.0.0"'
       }
     }
     stage('Install dependencies') {
       steps {
         sh '${BUNPATH}/bun install'
       }
     }
   }
 }
