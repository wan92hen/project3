 properties([ [ $class: 'ThrottleJobProperty',
                categories: ['metersphere'], 
                limitOneJobWithMatchingParams: false,
                maxConcurrentPerNode: 1,
                maxConcurrentTotal: 1,
                paramsToUseForLimit: '',
                throttleEnabled: true,
                throttleOption: 'category' ] ])

pipeline {
    agent {
        node {
            label 'metersphere'
        }
    }
    options { quietPeriod(600) }
    stages {
        stage('DEBUG') {
            steps {
                echo "DEBUG Started"
                sleep 100
                echo "DEBUG Ended"
            }
        }
    }
}
