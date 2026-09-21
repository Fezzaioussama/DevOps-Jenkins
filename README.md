# DevOps-Jenkins

> Placeholder repository — created for Jenkins CI/CD work that hasn't been started.

**This repository contains no code.** Its entire contents are this README, a
`.gitignore`, and an MIT `LICENSE`. There is no `Jenkinsfile`, no pipeline
configuration, and no application.

It's recorded here plainly so nobody clones it expecting a working Jenkins
setup.

## If you're picking this up

A Jenkins pipeline repo would normally start with a `Jenkinsfile` at the root:

```groovy
pipeline {
    agent any
    stages {
        stage('Build')  { steps { sh 'make build' } }
        stage('Test')   { steps { sh 'make test'  } }
        stage('Deploy') { steps { sh 'make deploy' } }
    }
    post {
        always { junit 'reports/**/*.xml' }
    }
}
```

## Meanwhile

Working CI examples do exist in the account, both using GitHub Actions rather
than Jenkins:

- **[scafolding](https://github.com/Fezzaioussama/scafolding)** — Makefile +
  pytest + pylint + GitHub Actions, the most complete of the two.
- **[Test_tuto](https://github.com/Fezzaioussama/Test_tuto)** — the same idea,
  smaller.

## License

MIT — see [`LICENSE`](LICENSE).
