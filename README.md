# Example with 'mavenDeployer' API

This example project demonstrates how to use Gradle's "maven" plugin ("mavenDeployer" API) to publish to:
 - JFrog Cloud Artifactory, see artifacts
 - JFrog Bintray

## Usage

### Bintray

To publish to Bintray:
 - export BINTRAY_USER and BINTRAY_API_KEY env variables
 - run ```./gradlew uploadArchives -i```
 - see published artifacts: https://linkedin.jfrog.io/linkedin/test-repo/com/linkedin/sample/gradle-mavenDeployer-example/    

### JFrog Cloud Artifactory

To publish to JFrog Cloud Artifactory:
 - comment out repo 2 in ```build.gradle``` file
 - export MVN_DEPLOY_USER and MVN_DEPLOY_KEY  env variables
 - run ```./gradlew uploadArchives -i```
 - see published artifacts: https://linkedin.bintray.com/test-repo/com/linkedin/sample/gradle-mavenDeployer-example/