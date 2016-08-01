# Image for testing Ansible Playbooks
This image provides a simple mechanism for testing ansible playbooks. The image comes with a standard ubuntu image with ssh enabled and a non-root user `ubuntu`.

**WARNING**
This is a test image for Ansible playbooks
**THIS IMAGE IS NOT TO BE USED IN PRODUCTION**

# Usage
To run the image for use with Ansible run:
```bash
$ docker run -d -P speyside/ansible-test
```
This will run the container in the background and accept ssh connections. Connections can be established for user `ubuntu` with password `ubuntu`. SSH key authentication can be used.

To retrieve the SSH private key authorized for this image, run the following command:
```bash
$ docker logs <container_name>
```
