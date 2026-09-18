```text
Option	Meaning
--no-audit	Skip vulnerability audit
--no-fund	Skip funding messages
--omit=dev	Skip devDependencies

For your React multi-stage Dockerfile, --no-audit --no-fund is mainly about making the build cleaner/faster, while
the actual production image is the NGINX stage containing only the React build files.

```
```text
dependencies = needed to run the application
devDependencies = needed to develop/test/build the application
--production / --omit=dev = install only what is needed to run.
```



