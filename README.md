# MNIST with Docker

## Starting up Vagrant, running Docker and following logs

* Create a terminal in vg-mnist
* Run `vagrant up` to set up Vagrant and install Docker
* The Vagrantfile itself also serves as the script to build the Dockerfile and run the Docker container directly, so no additional script is required.
* Once the VM is up, run `vagrant ssh` to get into the VM.
* To see the outputs in real time from the logs, type `docker logs --follow pytorch-mnist`
