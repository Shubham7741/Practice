pipeline {
    agent any
    parameters {
      string(name: 'HOSTNAME', defaultValue: '', description: 'hostname of the server')
      choice(name: 'OSVER', choices: ['2016', '2019'], description: '')
    }
    options {
        // Timeout counter starts AFTER agent is allocated
        //timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('VMBuild') {
            steps {
                echo 'Hello World'
                echo "OS Version of the server is ${params.VERSION}"
                echo 'Hostname is ${params.HOSTNAME}'
            }
        }
    }
}
