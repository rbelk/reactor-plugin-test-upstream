job('reacting/up') {
    deliveryPipelineConfiguration("up", "upper")
    scm {
        git {
            remote {
                url('https://github.com/rbelk/reactor-plugin-test-upstream')
            }
        }
    }
    wrappers {
        deliveryPipelineVersion('1.0.0.\$BUILD_NUMBER', true)
    }
    publishers {
        downstreamParameterized {
            trigger('reacting/down', 'SUCCESS', true) {

            }
        }
    }
}

/*node {
	
	println "pretend to build...";

	step([$class: 'FireEventStep', eventName: 'build', properties: """version=1.0"""]);
}
**/
