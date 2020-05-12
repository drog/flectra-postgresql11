# Instructions
This image is based from ubuntu image obtained from original repository https://gitlab.com/flectra-hq/flectra/-/tree/master/setup/docker

Docker image found in https://hub.docker.com/r/drog/flectra-postgres11

Commit `41b14aa996c4535ebfe09993678d453cc2b8ed84` is v1.6.4 https://gitlab.com/flectra-hq/flectra/-/commits/v1.6.4
- Build base image: `$ docker build -t flectra-base -f base/Dockerfile .`
- Build flectra image: `$ docker build -t flectra --build-arg BASE_IMAGE=flectra-base --build-arg GITLAB_COMMIT=41b14aa996c4535ebfe09993678d453cc2b8ed84 -f flectra/Dockerfile .`

# Versions
- v1.6.3: `80dcc24416e4d1a66b90e75f48f2ce9a3442a1c5`
- v1.6.4: `41b14aa996c4535ebfe09993678d453cc2b8ed84`