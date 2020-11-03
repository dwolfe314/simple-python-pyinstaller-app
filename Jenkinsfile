pipeline {
    agent any
    stages {
        stage('Stage 1') {       
            steps {
                echo 'Hello Python World'
                sh 'python3 -m py_compile sources/add2vals.py sources/calc.py'
            }
        }
    }
}
