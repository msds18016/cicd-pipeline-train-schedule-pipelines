pipeline{
  agent any
  stages {
    stage {'Build'}{
	  steps {
	    echo "Building the code"
		sh '.gradle build --no-daemon'
		archiveArtifacts artifacts: 'dist/trainSchedule.zip'
	  }
	}
  }
}
