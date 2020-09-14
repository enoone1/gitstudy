import hudson.model.*;

pipeline{

    agent  none

    stages{

        stage('1'){

            parallel{

                stage('Branch A'){

                    stages{

                        stage('1-1'){

                            steps{
                                echo ''
                            }
                        }

                        stage('1-2'){

                            steps{
                                echo ''
                            }
                        }
                    }
                }

                stage('Branch B'){

                    steps{
                        echo "On Branch B"
                    }
                }
            }
        }
    }
}