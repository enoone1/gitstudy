import hudson.model.*;

pipeline{

    agent {label 'lw'}

    stages{

        stage('Testing'){

            parallel{

                stage('Branch A'){

                    stages{

                        stage('A-1'){

                            steps{
                                echo 'A-1 testing'
                            }
                        }

                        stage('A-2'){

                            steps{
                                echo 'A-2 testing'
                            }
                        }
                    }
                }

                stage('Branch B'){
                
                stages{

                    stage('B-1'){

                            steps{
                                echo 'B-1 testing'
                            }
                        }

                        stage('B-2'){

                            steps{
                                echo 'B-2 testing'
                            }
                        }
                        }
                }
            }
        }
    }
}
