publishers {
    buildPipelineTrigger('downer') {
        parameters {
            propertiesFile('env.${BUILD_NUMBER}.properties')
        }
    }
}

node {
	
	println "pretend to build...";

	step([$class: 'FireEventStep', eventName: 'build', properties: """version=1.0"""]);
}
