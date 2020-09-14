node { 
    
     try {
        stage('Building') {
            echo "Building project2 files"
            error "building error"
        }
        
     } catch(e) {
            currentBuild.result = 'FAILURE'
     } finally {
            if (!currentBuild.result)
                currentBuild.result = currentBuild.currentResult
     }
    
    stage('Testing') {
            echo "Testing project2 files" 
        }
    stage('Depolying') {
             echo "Deploying project2 files" 
        }
 }
