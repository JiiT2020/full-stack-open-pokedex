


# nimeä .yml:ksi jos tätä hello.yml:ää vielä tarvitsee







# This is a basic workflow to help you get started with Actions

name: Hello World

# Controls when the workflow will run
on:
  # Triggers the workflow on push or pull request events but only for the master branch
  push:
    branches: 
    - master


# A workflow run is made up of one or more jobs that can run sequentially or in parallel
jobs:
  # This workflow contains a single job called "build"
  hello_world_job:
    # The type of runner that the job will run on
    runs-on: ubuntu-18.04

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:

      # Runs a set of commands using the runners shell
      - name: Say hello
        run: |
          echo "Hello World!"
      
      # Runs a set of commands using the runners shell
      - name: Now it is
        run: date
        
              # Runs a set of commands using the runners shell
      - name: Directory content
        run: ls -l

