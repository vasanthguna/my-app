node{
   stage('SCM Checkout'){
     git 'https://github.com/damodaranj/my-app.git'
   }
   stage ('Copy data from web server'){
    sshagent(['root']){
        sh'ssh -o StrictHostKeyChecking=no ubuntu@172.31.25.132'
        sh'scp /var/lib/jenkins/workspace/helloworld/* ubuntu@172.31.25.132:/var/www/html'
       sh' 
    }
}
}
