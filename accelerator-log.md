# Accelerator Log

## Options
```json
{
  "devWorkloadType" : "web-dev",
  "gitBranch" : "main",
  "gitRepo" : "https://github.com/tmm-tanzu/spring-sensors-rabbit.git",
  "localPath" : "/Users/taaron/tap/code-repos/spring-sensors-rabbit",
  "prodWorkloadType" : "web",
  "projectName" : "spring-sensors-rabbit",
  "publisherRepository" : "index.docker.io/springdeveloper/spring-sensors-publisher",
  "sourceImage" : "gcr.io/taaron-1/spring-sensors-app-source",
  "title" : "Tanzu Sensor Database"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml matched [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml matched [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml matched [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┗ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [config/workload.yaml, demo/**, src/main/resources/application.yaml, catalog/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [GITREPO->https://github.com/t...(truncated), main->main, WORKLOADTYPE->web]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [Tiltfile]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [DEVWORKLOADTYPE->web-dev]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [src/main/resources/application.yaml]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml matched [src/main/resources/application.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [Tanzu Sensor Database->Tanzu Sensor Databas...(truncated)]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[4].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [demo/publisher-deployment.yaml, demo/publisher-image.yaml]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml matched [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml matched [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [dev.local/spring-sensors-publisher->index.docker.io/spri...(truncated)]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[5].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [.vscode/settings.json]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json matched [.vscode/settings.json] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [.vscode/settings.json] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┗ ┗ ┗ ┗  Info Will replace [SOURCEIMAGE->gcr.io/taaron-1/spri...(truncated), LOCALPATH->/Users/taaron/tap/co...(truncated)]
┃ ┃ ┏ engine.transformations[0].merge.transformations[1] (UniquePath)
┃ ┗ ┗ Debug Multiple representations for path '.vscode/settings.json', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```
