/*
job('up/upper') {
	deliveryPipelineConfiguration("CI", "Deploy")

    	wrappers {
        	buildName('\$PIPELINE_VERSION')
    	}
    
        publishers {
        	downstreamParameterized {
            		trigger('down/downer', 'SUCCESS', true) {
            		}
        	}
    	}
}
**/
return False;
/*node {
	
	println "pretend to build...";

	step([$class: 'FireEventStep', eventName: 'build', properties: """version=1.0"""]);
}
**/
