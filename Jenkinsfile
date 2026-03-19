pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                // Get some code from a GitHub repository
               // git url: 'https://github.com/v484816/MyRepo2', branch: 'main'
                
            }
        }
        stage('HCL DevOps Test UI script execution phase') {
            steps {
                echo("************************** Web UI Test - HCL DevOps Test UI Start **************************")
                step([$class: 'RTWProductHelper', configfile: '', exportReportFileName: '', exportReportFolder: 'D:\\Jenkins_rep', exportReportFormat: 'HTML', exportReportType: 'unified', exportReportUsage: true, exportstatreportlist: '', exportstats: '', exportstatsformat: '', exportstatshtml: '', imports: '', imsharedloc: 'C:\\Program Files\\HCL\\HCLIMShared', labels: '', name: 'Jenkins_Test_UI', overwrite: 'true', project: 'google', protocolinput: '', publish: '', publishfor: '', publishreports: '', quiet: 'false', results: '', suite: 'test.testsuite', swapdatasets: '', usercomments: '', varfile: '', vmargs: '', workspace: 'D:\\workspace2'])
                echo("************************** Web UI Test - HCL DevOps Test UI End **************************")

            }
        }
        
    }
}


