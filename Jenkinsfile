pipeline {
  agent any

  stages {
    stage('Clone Repository') {
        when {
            branch 'main'
        }
        steps {
            git 'https://github.com/RajagopalAswin1994/automate-jenkins-pipeline-djangoapp.git'
        }
    }

//     stage('Build') {
//       steps {
//         sh 'pip install pyinstaller'
//         sh 'pyinstaller --name=profileapp --onefile '
//       }
//     }

//     stage('Sonarqube Analysis') {
//       steps {
//         withSonarQubeEnv('sonarqube') {
//           sh 'sonar-scanner'
//         }
//       }
//     }

//     stage('Build Docker Image') {
//       steps {
//         sh 'docker build -t <docker_image_name> .'
//       }
//     }

//     stage('Deploy to EC2') {
//       steps {
//         sshagent(['<remote_server_credential>']) {
//           sh '''
//             ssh <remote_server_ip> << EOF
//               sudo docker stop <container_name> || true
//               sudo docker rm <container_name> || true
//               sudo docker rmi <docker_image_name> || true
//             EOF
//           '''
//           sh '''
//             scp -o StrictHostKeyChecking=no <docker_image_name> <remote_server_ip>:~
//             ssh <remote_server_ip> << EOF
//               sudo docker run -d -p <port>:<port> --name <container_name> <docker_image_name>
//             EOF
//           '''
//         }
//       }
//     }

//     stage('Configure Grafana and Prometheus') {
//       steps {
//         sshagent(['<remote_server_credential>']) {
//           sh '''
//             ssh <third_ec2_ip> << EOF
//               sudo docker-compose up -d
//             EOF
//           '''
//         }
//       }
//     }
//   }

//   post {
//     always {
//       junit '**/test-results/*.xml'
//     }
  }
}
