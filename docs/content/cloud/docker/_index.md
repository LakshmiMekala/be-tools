---
title: Docker
weight: 4220
# chapter: true
# pre: "<i class=\"fas fa-cloud\" aria-hidden=\"true\"></i> "
---

## Dockerize TIBCO BusinessEvents

Using the scripts provided at the TIBCO BusinessEvents GitHub repository, you can containerize and run a TIBCO BusinessEvents application by using Docker.

Docker provides a way to run applications securely isolated in a container, packaged with all its dependencies and libraries. Your application can run in any environment as all the dependencies are already present in the image of the application. For details about Docker, see Docker Documentation.

A TIBCO BusinessEvents application comprises a common TIBCO BusinessEvents runtime and project (application) specific TIBCO BusinessEvents code running inside the TIBCO BusinessEvents runtime. Thus to containerize a TIBCO BusinessEvents application, TIBCO BusinessEvents software archive and application archive are included in the Docker image.
Docker Scripts with BusinessEvents
TIBCO BusinessEvents provides the following scripts for building images of TIBCO BusinessEvents application and its components at cloud/docker/bin:

    build_app_image - Script to build the Docker image for your TIBCO BusinessEvents application.
    build_rms_image - Script to build the Docker image for RMS.
    build_teagent_image - Script to build the Docker image for TIBCO BusinessEvents Enterprise Administrator Agent.

These scripts use the platform-specific Dockerfiles bundled with TIBCO BusinessEvents at cloud/docker/bin. For details about Dockerfiles provided with TIBCO BusinessEvents, see Dockerfile for TIBCO BusinessEvents.