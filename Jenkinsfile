pipeline
{
    agent any
    stages{
        stage('Build')
        {
            steps{
                sh 'g++ new.cpp'
                echo 'Build stage successful'
            }
        }
        stage('Test'){
            steps{
                sh './a.out'
                echo 'Test stage successful'
            }
        }
//         stage('Deploy'){
//             steps{
//                 echo 'Deployment successful'
//              }
//         }
    }
    post{
        failure{
            echo 'Pipeline failure'
        }
    }
}
