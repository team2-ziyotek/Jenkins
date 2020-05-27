pipeline {
    agent any
    stages {
        stage("Create our team members!") {
            steps {
                sh """
                    touch aziza
                    touch iroda
                    touch nozima
                    touch kamola
                    touch madina
                    touch jesse
                    touch o'ktamaka
                    touch cheick
                """
            } //steps 
        } //stage
        stage("Run ziyotek") {
            steps {
                sh """
                    python ziyotek.py
                """
            } //steps
        } //stage
        stage("Run game.py") {
            steps {
                sh """
                    python game.py
                """
            } //steps
        } //stage
    } //stages
    post {
        always {
            sh """
                rm -f aziza
                rm -f iroda
                rm -f nozima
                rm -f kamola
                rm -f madina
            """
        }
    }
} //pipeline