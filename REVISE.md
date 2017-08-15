this readme is about what we revise the bbs to support the k8s runtime.
As a toast, we made the following work:
- first we implement a k8s service which receive the requests from lrp or task.(done)
- second we revise startInstanceRange in desired_lrp_handlers.go to do the container setup job.(done)
- third we revise the handlers.go file to add k8sclient in handlers.New() method;(done)
- forth we need to revise the cmd/main.go file to create a k8sclient and add the client to the handlers(wait to be done)
- fifth we need to upload all the code to diego relaese to create a new portable release(wait to be done)
- finally we need to deploy the new release to the cf-release to create a new cf-release(wait to be done)