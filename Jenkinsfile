node(){
    stage("git clone"){
        checkout scm
    }    
    stage("build-upload artifacts"){
        sh "mvn clean package"
    }
//     stage("copying required files"){
//         sh "scp -o StrictHostKeyChecking=no target/*.war root@docker-master:/inet/projects"
//         sh "scp -o StrictHostKeyChecking=no Dockerfile root@docker-master:/inet/projects"
//         sh "scp -o StrictHostKeyChecking=no kubernetes-deployment.yml root@k8smaster:/inet/projects"
//    }


//     stage("Building the Docker image"){ 
//         sh 'docker build -t bookstore.app.v1.$BUILD_ID /inet/projects'
//         sh 'docker tag bookstore.app.v1.$BUILD_ID steju480/bookstore.app.v1.$BUILD_ID'
//         sh 'docker tag bookstore.app.v1.$BUILD_ID steju480/bookstore.app.v1'
//     }
//     stage("Docker image push"){
//         withCredentials([usernamePassword(credentialsId: 'dockerhub', passwordVariable: 'password', usernameVariable: 'user')]) {
//             sh "docker login -u ${user} -p ${password}"
//             sh 'docker login -u steju480 -p Steju@1997'
//             sh 'docker push steju480/bookstore.app.v1.$BUILD_ID'
//             sh 'docker push steju480/bookstore.app.v1'
//             sh 'docker rmi steju480/bookstore.app.v1.$BUILD_ID'
//             sh 'docker rmi steju480/bookstore.app.v1' 
//             sh 'docker rmi bookstore.app.v1.$BUILD_ID'
//           }                        
//       }  
//      stage("deploying the app"){     
//         sh 'aws eks --region <region-code> update-kubeconfig --name mycluster'
//         sh "kubectl delete -f /inet/projects/kubernetes-deployment.yml"
//         sh "kubectl create -f /inet/projects/kubernetes-deployment.yml"

}      
