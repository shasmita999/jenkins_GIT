pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                // Get some code from a GitHub repository
                git url: 'https://github.com/v484816/MyRepo2', branch: 'main'
                
            }
        }
        stage('Functional Test - HCL OneTest UI') {
            steps {
                echo("************************** Functional Test - HCL OneTest UI Start **************************")
                step([$class: 'RTWProductHelper', configfile: '', exportReportFileName: '', exportReportFolder: 'D:\\Jenkins_rep', exportReportFormat: 'HTML', exportReportType: 'unified', exportReportUsage: true, exportstatreportlist: '', exportstats: '', exportstatsformat: '', exportstatshtml: '', imports: '', imsharedloc: 'C:\\Program Files\\HCL\\HCLIMShared', labels: '', name: 'Jenkins_HOT_UI', overwrite: 'true', project: 'GIT_Jenkins', protocolinput: '', publish: '', publishfor: '', publishreports: '', quiet: 'false', results: '', suite: 'Demo.testsuite', swapdatasets: '', usercomments: '', varfile: '', vmargs: '', workspace: 'D:\\HCL_Workspace_10_5_3_jenkins'])
                echo("************************** Functional Test - HCL OneTest UI End **************************")

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}


