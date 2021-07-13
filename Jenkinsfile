pipeline{
    agent any
    stages{
        stage("Build"){
            when {
                branch 'develop'
            }
            steps{
                echo "build with maven"
            }
        }
        stage("Upload to Nexus"){
            when {
                branch 'develop'
            }
            steps{
                echo "upload to nexus"
            }
        }
        stage("Deploy to dev"){
            when {
                branch 'develop'
            }
            steps{
                echo "deploy to dev"
            }
        }
        stage("Deploy to test"){
            when {
                branch 'test'
            }
            steps{
                echo "Deploy to Test"
            }
        }
        stage("Deploy to prod"){
            when {
                branch 'master'
            }
            steps{
                echo "Deploy to Production"
            }
        }
    }
}
