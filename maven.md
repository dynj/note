
## Tricks
### How to time the different stages of maven execution

```bash
export MAVEN_OPTS="-Dorg.slf4j.simpleLogger.dateTimeFormat=HH:mm:ss,SSS \
                   -Dorg.slf4j.simpleLogger.showDateTime=true" 
mvn test

```
results in
```bash
MAVEN_OPTS="-Dorg.slf4j.simpleLogger.dateTimeFormat=HH:mm:ss,SSS -Dorg.slf4j.simpleLogger.showDateTime=true" mvn test
17:06:07,330 [INFO] Scanning for projects...
17:06:07,447 [INFO] 
17:06:07,447 [INFO] ------------------------------------------------------------------------
17:06:07,448 [INFO] Building bimble-server 0.0.1-SNAPSHOT
17:06:07,448 [INFO] ------------------------------------------------------------------------
17:06:07,747 [INFO] 
17:06:07,748 [INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ bimble-server ---
```
