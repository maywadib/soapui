node {
        stage('Checkout') {
            git url: 'https://github.com/maywadib/soapui.git',  branch: 'master'
            echo '****************CHECKOUT SUCCESSFUL****************'
        }
       

       stage('Docker Deploy') {
            bat 'cd "C:/Program Files/SmartBear/SoapUI-5.5.0/bin"'
			bat 'testrunner.bat -sSampleTestSuite -r -j C:/Mayur/SoapUI/projects/SampleProject.xml'
			echo '****************DOCKER DEPLOY SUCCESSFUL****************'
        }

}