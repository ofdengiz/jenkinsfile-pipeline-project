# jenkinsfile-pipeline-project

A minimal Jenkins declarative pipeline that compiles and runs a single Java file. Reference for Jenkinsfile syntax — stages, steps, shell execution.

**Stack:** Jenkins · Groovy · Java

## Pipeline

```groovy
pipeline {
  agent any
  stages {
    stage('build') { sh 'javac Hello.java' }
    stage('run')   { sh 'java Hello' }
  }
}
```

## For my current Jenkins / CI work

See **[`ofdengiz/petclinic-microservices-with-db`](https://github.com/ofdengiz/petclinic-microservices-with-db)** — end-to-end Jenkins CI/CD with multi-branch pipelines, ECR, Rancher-managed EKS, and Prometheus + Grafana monitoring.
