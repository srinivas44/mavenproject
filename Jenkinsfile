node {
    stage('SCM CheckoutNak'){
	git 'https://github.com/srinivas44/mavenproject.git'
      }

    stage('Compile-Package'){
     sh 'mvn package'
     }
}
