# Dockerfile Bug Report

This repository demonstrates a common error encountered when building Docker images: issues with file paths and dependencies. The original Dockerfile (`Dockerfile`) fails to build because of issues.  The solution is provided in the file `Dockerfile_fixed`. 

## Bug Description
The initial `Dockerfile` fails to build because of an issue with the `COPY` instruction's file path. This leads to a failure to install the required Python packages and thus the application fails to start in the container.

## Solution
The corrected `Dockerfile` (`Dockerfile_fixed`) addresses this by ensuring that all required files, including the `requirements.txt` are correctly located and copied before the installation of dependencies. 