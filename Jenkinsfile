node {
    def PYTHON = 'C:\\Users\\APOORBA\\AppData\\Local\\Programs\\Python\\Python314\\python.exe'
    try {
        stage('checkout code') {
            checkout scm
        }

        stage('show python version') {
            bat "${PYTHON} --version"
        }

        stage('run python program') {
            bat "${PYTHON} extract_data.py"
        }
    }
    catch(err) {
        echo 'pipeline failed: ${err}'
    } 
}