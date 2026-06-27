pipeline{

     agent any

     stages{

        stage('Restore'){
            when{
                anyOf{
                    branch 'main'
                }
            }
            streps{
                bat 'dotnet restore'
            }
        }stage('Build'){
            when{
                anyOf{
                    branch 'main'
                }
            }
            streps{
                bat 'dotnet build'
            }

        }stage('Test'){
            when{
                anyOf{
                    branch 'main'
                }
            }
            stages{
                bat 'dotnet test'
            }
        }











    }









}
