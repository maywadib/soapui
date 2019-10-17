node {
        stage('Checkout') {
            git url: 'https://github.com/maywadib/soapui.git',  branch: 'master'
            echo '****************CHECKOUT SUCCESSFUL****************'
        }
       

       stage('Docker Deploy') {
            def docker = 'docker'
            //sh '(docker stop dev-product-service-container || true) && (docker rm dev-product-service-container || true) && (docker rmi pms-product-service-app || true)'
            //sh 'docker build ./ -t pms-product-service-app && docker run -p 8006:8006 -e "SPRING_PROFILES_ACTIVE=dev" --name dev-product-service-container --link dev-eureka-container pms-product-service-app'
            //sh 'docker ps'
			echo '****************DOCKER DEPLOY SUCCESSFUL****************'
        }

}