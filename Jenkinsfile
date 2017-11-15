node (){
  stage 'Build and Test'
  env.PATH = "${tool 'M3'}/bin:${env.PATH}"
  checkout scm
  sh 'mvn clean package'
}
