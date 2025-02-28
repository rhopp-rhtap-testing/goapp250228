# Trusted Application Pipeline Software Template

This application, **goapp250228**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/rhopp-rhtap-testing/goapp250228 ](https://github.com/rhopp-rhtap-testing/goapp250228 ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/rhopp-rhtap-testing/goapp250228-gitops ](https://github.com/rhopp-rhtap-testing/goapp250228-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |
| **rhtap-app-ci** | The namespace used for CI workloads |
| **rhtap-app-development** | The default application during development. Every build will be deployed to this namespace for testing. |
| **rhtap-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/rhopp-rhtap-testing/goapp250228-gitops ) in the components/goapp250228/overlays/stage directory |
| **rhtap-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/rhopp-rhtap-testing/goapp250228-gitops ) in the components/goapp250228/overlays/prod directory |