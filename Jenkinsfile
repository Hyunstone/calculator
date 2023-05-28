pipeline { 
     agent any 
     stages { 
          stage("Compile") { 
               steps { 
                    sh "sleep 5"
                    sh "./gradlew compileJava" 
               } 
          }
            stage("Build") {
                         steps {
                              sh "./gradlew build"
                         }
                    }

          stage("Unit test") { 
               steps { 
                    sh "./gradlew test" 
               } 
          } 
     } 
} 
