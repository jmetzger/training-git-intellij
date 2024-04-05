# Kann ich eine Stage manuell starten ? 

## So geht's ;o) 

```yaml
stages:          # List of stages for jobs, and their order of execution
  - build
  - test

build-job:       # This job runs in the build stage, which runs first.
  stage: build
  script:
    - echo "Compiling the code..."
    - echo "Compile complete."

unit-test-job:   # This job runs in the test stage.
  stage: test    # It only starts when the job in the build stage completes successfully.
  script:
    - echo "Running unit tests... This will take about 60 seconds."
    - sleep 60
    - echo "Code coverage is 90%"
  when: manual 

```

## Beispiel: Deploy läuft erst, wenn Testing erfolgreich durchgeführt wurde 

  * d.h. händisch gestartet und erfolgreich ausgeführt wurde.
  * Keyword ist hier: allow_failure: false

```
stages:          # List of stages for jobs, and their order of execution
  - build
  - test
  - deploy

build-job:       # This job runs in the build stage, which runs first.
  stage: build
  script:
    - echo "Compiling the code..."
    - echo "Compile complete."

unit-test-job:   # This job runs in the test stage.
  stage: test    # It only starts when the job in the build stage completes successfully.
  script:
    - echo "Running unit tests... This will take about 60 seconds."
    - sleep 10
    - echo "Code coverage is 90%"
  allow_failure: false
  when: manual 

deploy-job:   # This job runs in the test stage.
  stage: deploy    # It only starts when the job in the build stage completes successfully.
  script:
    - echo "Now deploying "
    - echo "Deployment done "

```


