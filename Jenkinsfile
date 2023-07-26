pipeline{
    agent any
        stages{
                stage ('1-clone'){
                    steps{
                        checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'groupgit', url: 'https://github.com/AppGroup2/jenkinsproject2.git']])

                        }   
                    }
                stage('2-Group Parallel job'){
                    parallel{
                        stage('Titi-sub-job-1'){
                            steps{
                                sh 'lscpu'
                                sh 'echo $SHELL'
                            }
                        }
                        stage('Baba'){
                            steps{
                            sh 'sudo systemctl status jenkins'
                            }
                        }
                    }
                }
                stage('3-Group Parallel job'){
                    parallel{
                        stage('Aubin'){
                            steps{
                                sh 'ls'
                            }
                        }
                        stage('IyaAfeez'){
                            steps{
                                sh 'pwd'
                            }
                        }
                    }
                }
                stage('4-Group Parallel job'){
                    parallel{
                        stage('Olujimi'){
                            steps{
                                sh 'lscpu'
                            }
                        }
                        stage('Kayode'){
                            steps{
                                sh 'pwd'
                            }
                        }
                        stage('Christian'){
                            steps{
                                sh 'whoami'
                            }
                        }
                    }
                }
    

            }   



    }