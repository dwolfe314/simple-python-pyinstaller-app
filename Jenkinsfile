pipeline {
    agent none
    stage('Build') {       
        steps {
            sh 'python3 -m py_compile sources/add2vals.py sources/calc.py'
        }
    }
}
