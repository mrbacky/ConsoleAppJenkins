pipeline {
	agent any
	triggers {
		cron("0 * * * *")
	}
	stages{
		stage("Build"){
			steps{
				sh "dotnet build ConsoleAppJenkins/ConsoleAppJenkins.csproj"
			}
		}
		stage("Test"){
			steps{
				sh "dotnet test ConsoleAppJenkins/ConsoleAppJenkins.csproj"
			}
		}
	}
}