# javascript-app-4

### **Key**:

* Host: Windows 10
* IDE: Visual Studio Code v1.78.2
* Hypervisor: VirtualBox 6.1
* Guest: Ubuntu 22.04
* JavaScript
* Node.js v19.9.0
* Docker v20.10.24, build 297e128

### **Summary**:
This project builds a simple "Hello, word!" application using node.js and Docker. 

### **Instructions**:

1. Build the Docker file

<pre>
sudo docker build . -t js-app-4:1.0
</pre>

2. View the list of images

<pre>
sudo docker image ls
</pre>

3. Run the image

<pre>
sudo docker run -p 3000:3000 -d js-app-4:1.0
</pre>

-p : specify ports host:guest \
-d : run in detached mode (background)

4. View running containers

<pre>
sudo docker ps
</pre>

5. View app in browser

Port forwarding is enabled between the VM and the host. The Docker container will route to from its port 3000 to the guest port 3000 and finally to the host port 3000. In the browser search localhost:3000. 


### **References**:

* https://nodejs.org/en/docs
* https://docs.docker.com/