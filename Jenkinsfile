pipeline {
    agent any 
    stages {
        stage('Paso 1') {
            steps {
                parallel(
                  first: {
                    echo "${currentBuild.number}: ¡Hola ${params.NAME} desde el primer paso!"
                    sleep 2
                  },
                  second: {
                    echo "${currentBuild.number}: ¡Hola ${params.NAME} desde el segundo paso!"
                    sleep 2
                  }
                )
            }
        }
    }
}
