<a id="top"></a>

<p style="font-size: 24px;"><img src="./qct-icons/transform-logo.svg" style="margin-right: 15px; vertical-align: middle;"></img><b>Code Transformation Summary by Amazon Q </b></p>
<p><img src="./qct-icons/transform-variables-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Lines of code in your application: 2039 <p>
<p><img src="./qct-icons/transform-clock-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Transformation duration: 17 min(s) <p>
<p><img src="./qct-icons/transform-dependencies-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Planned dependencies replaced: 3 of 6 <p>
<p><img src="./qct-icons/transform-dependencyAnalyzer-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Additional dependencies added: 13 <p>
<p><img src="./qct-icons/transform-smartStepInto-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Planned deprecated code instances replaced: 0 of 0 <p>
<p><img src="./qct-icons/transform-listFiles-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Files changed: 4 <p>
<p><img src="./qct-icons/transform-build-dark.svg" style="margin-bottom: 1px; vertical-align: middle;"></img> Build status in Java 17: <span style="color: #00CC00">SUCCEEDED</span> <p>

### Table of Contents

1. <a href="#build-log-summary">Build log summary</a> 
1. <a href="#planned-dependencies-replaced">Planned dependencies replaced</a> 
1. <a href="#additional-dependencies-added">Additional dependencies added</a> 
1. <a href="#deprecated-code-replaced">Deprecated code replaced</a> 
1. <a href="#other-changes">Other changes</a> 
1. <a href="#all-files-changed">All files changed</a> 
1. <a href="#next-steps">Next steps</a> 


### Build log summary <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="build-log-summary"></a>

Amazon Q successfully built the upgraded code in Java 17. Here is a relevant snippet from the build log. To view the full build log, open [`buildCommandOutput.log`](./buildCommandOutput.log)

```
The Maven build was successful in 21 seconds. It compiled 29 Java source files, generated component and Sling model code, and created various resources under ui.apps and core. There were deprecation warnings during compilation. No tests were executed.
```


### Planned dependencies replaced <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="planned-dependencies-replaced"></a>

Amazon Q updated the following dependencies that it identified in the transformation plan

| Dependency | Action | Previous version in Java 8 | Current version in Java 17 |
|--------------|--------|--------|--------|
| `jakarta.servlet:jakarta.servlet-api` | Added | - | 6.1.0 |
| `junit:junit` | Removed | 4.13.1 | - |
| `org.apache.logging.log4j:log4j-api` | Added | - | 2.23.1 |

### Additional dependencies added <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="additional-dependencies-added"></a>

Amazon Q updated the following additional dependencies during the upgrade

| Dependency | Action | Previous version in Java 8 | Current version in Java 17 |
|--------------|--------|--------|--------|
| `com.fasterxml.jackson.core:jackson-databind` | Updated | 2.12.7.1 | 2.17.2 |
| `net.sf.saxon:Saxon-HE` | Updated | 9.7.0-15 | 12.5 |
| `org.apache.commons:commons-lang3` | Updated | 3.9 | 3.14.0 |
| `org.apache.commons:commons-text` | Updated | 1.10.0 | 1.12.0 |
| `org.apache.felix:org.apache.felix.http.servlet-api` | Updated | 1.1.2 | 3.0.0 |
| `org.apache.logging.log4j:log4j-core` | Updated | 2.17.1 | 2.23.1 |
| `org.apache.maven.plugins:maven-antrun-plugin` | Updated | 3.0.0 | 3.1.0 |
| `org.apache.maven.plugins:maven-compiler-plugin` | Updated | 3.8.1 | 3.13.0 |
| `org.apache.maven.plugins:maven-resources-plugin` | Updated | 3.1.0 | 3.3.1 |
| `org.apache.sling:org.apache.sling.api` | Updated | 2.25.4 | 2.27.6 |
| `org.apache.sling:org.apache.sling.models.api` | Updated | 1.3.6 | 1.5.4 |
| `org.codehaus.mojo:exec-maven-plugin` | Updated | 3.0.0 | 3.3.0 |
| `org.junit.jupiter:junit-jupiter-api` | Updated | 5.3.2 | 5.10.3 |

### Deprecated code replaced <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="deprecated-code-replaced"></a>

Amazon Q replaced the following instances of deprecated code. An instance with 0 files
changed indicates Amazon Q wasn't able to replace the deprecated code.

| Deprecated code | Files changed |
|----------------|----------------|


### Other changes <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="other-changes"></a>



### All files changed <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="all-files-changed"></a>

| File | Action |
|----------------|--------|
| [pom.xml](../pom.xml) | Updated |
| [src/main/java/com/adobe/aem/compgenerator/javacodemodel/TestClassBuilder.java](../src/main/java/com/adobe/aem/compgenerator/javacodemodel/TestClassBuilder.java) | Updated |
| [src/main/java/com/adobe/aem/compgenerator/utils/CommonUtils.java](../src/main/java/com/adobe/aem/compgenerator/utils/CommonUtils.java) | Updated |
| [src/main/java/com/adobe/aem/compgenerator/utils/ComponentUtils.java](../src/main/java/com/adobe/aem/compgenerator/utils/ComponentUtils.java) | Updated |

### Next steps <a style="float:right; font-size: 14px;" href="#top">Scroll to top</a><a id="next-steps"></a>

1. Please review and accept the code changes using the diff viewer.If you are using a Private Repository, please ensure that updated dependencies are available.
1. 
1. In order to successfully verify these changes on your machine, you will need to change your project to Java 17. We verified the changes using [Amazon Corretto Java 17](https://docs.aws.amazon.com/corretto/latest/corretto-17-ug/what-is-corretto-17.html
) build environment.
1. If this project uses Maven CheckStyle, Enforcer, FindBugs or SpotBugs plugins, Q Code Transformation will disable those plugins when we build the project to verify proposed upgrades.