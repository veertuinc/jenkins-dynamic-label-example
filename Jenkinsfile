def LABEL = createDynamicAnkaNode(
  masterVmId: 'c0847bc9-5d2d-4dbc-ba6a-240f7ff08032',
  tag: 'base:port-forward-22:brew-git:jenkins:openjdk-1.8.0_242'
)

pipeline {
  agent {
    label "${LABEL}"
  }
  stages {
    stage('Begin parallel stage execution') {
      parallel {
        stage("parallel builder command1") {
          steps {
            echo "command1"
          }
        }
        stage("parallel builder command2") {
          steps {
            echo "command2"
          }
        }
        stage("parallel builder command3") {
          steps {
            echo "command3"
          }
        }
        stage("parallel builder command4") {
          steps {
            echo "command3"
          }
        }
      }
    }
  }
}