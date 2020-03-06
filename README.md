Dummy JPMS project to test [TINKERPOP-2347](https://issues.apache.org/jira/browse/TINKERPOP-2347).

Make sure Java 9+ is in use, then run:

```
mvn compile exec:java -Dexec.mainClass=com.acme.Main
```

Without the fix, this warning is emitted but the program still runs:
```
[WARNING] Can't extract module name from gremlin-shaded-3.3.11-SNAPSHOT.jar: Provider class com.fasterxml.jackson.core.JsonFactory not in module
```

When running from IDEA, the program doesn't run at all.

