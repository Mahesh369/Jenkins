pipeline{
		agent any
				stages{
					stage('One'){
							steps{
								echo "this is Mahesh. Helllo world!!!!"
								}
					}
					stage('Two'){
							steps{
								input('do you want to proceed?')
								}
					}
					stage('Three'){
							when{
									not {
											branch "master"
									}
								}
							steps{
								echo "Helllo world!!!!"
								}
							}
					stage('Four'){
							parallel{
									stage('Unit Test'){
													steps{
														echo "Running unit tests ...."
													}
									}
									stage('Integration Test'){
													steps{
														echo "Running unit tests ...."
													}
									}
							}
					}
			}
		}
