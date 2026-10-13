// pipeline {
//   agent any

//     stages {
//         stage('Build') {
//             steps {
//                 script {
//                     sh 'docker build -t my-app:latest -f dockerfile.dev .'
//                 }
//             }
//         }

//         stage('Test') {
//             steps {
//                 script {
//                     withEnv(['DOCKER_BUILDKIT=1']) {
//                         sh 'docker run -e CI=true my-app:latest npm run test'
//                     }
//                 }
//             }
//         }
//     }
// }