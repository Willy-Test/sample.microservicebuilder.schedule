@Library('MicroserviceBuilder') _
microserviceBuilderPipeline {
  image = 'microservice-schedule'
  mvnCommands = 'clean package -P security'
}

// Comment out mvnCommands to stop using the secured version of this microservice