pipeline{
agent any
stages{
stage("cloning the code"){
 steps{
 script{
     sh'git clone https://github.com/venkat0007/frontend-npm.git -b main'
     }
     }
     }
     stage ("building an image"){
     steps{
     script{
       sh'docker build -t forntend-npm:1 .'
       }
       }
       }
       stage("pushing the image to docker hub"){
       steps{
       script{
          sh'''
	  docker tag frontend-npm:1 venkat0007/frontend-npm:1
	  docker push venkat0007/forntend-npm:1'''
	  }
	  }
	  }
	  }
	  }



