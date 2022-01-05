env:
  STACK: java
  BUILD_TECH: java_maven
  
  on:
  push:
  # and the target with some regex to match specific  branch namess
    branches:
      - master
      - 'FEATURE-[0-9]-[0-9]-[0-9]-X-BRANCH'
      - '[0-9]_[0-9]_x'
      - '[0-9]-[0-9]-X-BRANCH'
