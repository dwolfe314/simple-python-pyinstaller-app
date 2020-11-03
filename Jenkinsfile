pipeline {
    agent any
    stages {
        stage('Build') {       
            steps {
                echo 'Build phase'
                sh 'python3 -m py_compile sources/add2vals.py sources/calc.py'
            }
        }
        stage ('Test') {
            steps {
                echo 'Test phase'
                sh 'py.test --junit-xml test-reports/results.xml sources/test_calc.py'
            }
        }
        stage ('Deliver') {
            steps {
                echo 'Deliver phase'
                sh 'pwd'
                sh 'whoami'
                sh '/home/dwolfe314/.local/bin/pyinstaller'
            }
        }
    }
}
