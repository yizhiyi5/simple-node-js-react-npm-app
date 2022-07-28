// pipeline {
//     agent {
//         docker {
//             image 'node:6-alpine' 
//             args '-p 3000:3000' 
//         }
//     }
//     stages {
//         stage('Build') { 
//             steps {
//                 sh 'npm install' 
//             }
//         }
//     }
// }

node {
	def mvnHome
	stage('拉取代码') {
    checkout([$class: 'GitSCM', branches: [[name: '*/test']], extensions: [], userRemoteConfigs: [[credentialsId: '2b610a7f-5a1a-4d0c-8f93-29aabe182c88', url: 'https://codeup.aliyun.com/6191d29d38b0ff04d2a421d4/huameng_safe_product/safe-product-web.git']]])
   }
}
