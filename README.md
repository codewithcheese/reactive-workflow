# Reactive workflow

Dynamic workflows built from reactive jobs for GitHub actions.

## How it works

The `setup` workflow calculates a DAG of jobs based on their input and output rules, and compiles a new workflow.

The compiled workflow is then pushed to a temporary branch with an `on: push` clause, causing it to be triggered 
immediately.

## Features
- Automatic loading and saving of input and output artifacts
- Automatic finalization of artifacts
- Load jobs from multiple source depending on org configuration 
- Generate documentation depending on jobs installed
- Generate tests harness for individual jobs
  - Harness expects input type and artifact, asserts output type and artifact










