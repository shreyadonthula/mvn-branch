@Library('shared-library2') _
pipeline{
    agent any
    stages{
         stage("build"){
            steps{
                script{
                    build()
                }
            }   
        } 
       stage("Test"){
            steps{
                script{
                    test()
                }
            }   
        }
	 stage("Package"){
            steps{
                script{
                    packaging.package()
                }
            }   
        }

	 stage("Git checkout SCM"){
            steps{
                script{
                   echo  'started git checkout...'
			
                }
            }   
        }
	 stage("Stages"){
            steps{
               
                echo "last stage"
             }
        }
    }   
}
