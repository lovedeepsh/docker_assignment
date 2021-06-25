DAY 1 Docker

Assignment 1
1. Use official shell script to install and configure Docker on your control machine. 

![Script](https://github.com/lovedeepsh/Docker_Assignment/blob/master/day1/script)

2. Start Docker service and check status of the same.
```
sudo systemctl status start docker.service
```
 
3. Enable Docker service to start at every machine reboot.
```
Sudo systemctl enable docker.service
```
 
4. Display Docker version. 
```
Docker --version
```
5. Configure non root user to run docker commands without sudo. 
```
sudo adduser love
sudo usermod -aG docker love
su – love
```


To verify : -
```
id -nG
```
6. Type docker on commandline and read output i.e containing related commands. 
```
docker
```
```
attach      Attach local standard input, output, and error streams to a running container
  build       Build an image from a Dockerfile
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  events      Get real time events from the server
  exec        Run a command in a running container
  export      Export a container's filesystem as a tar archive
  history     Show the history of an image
  images      List images
  import      Import the contents from a tarball to create a filesystem image
  info        Display system-wide information
  inspect     Return low-level information on Docker objects
  kill        Kill one or more running containers
  load        Load an image from a tar archive or STDIN
  login       Log in to a Docker registry
  logout      Log out from a Docker registry
  logs        Fetch the logs of a container
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  ps          List containers
  pull        Pull an image or a repository from a registry
  push        Push an image or a repository to a registry
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  rmi         Remove one or more images
  run         Run a command in a new container
  save        Save one or more images to a tar archive (streamed to STDOUT by default)
  search      Search the Docker Hub for images
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  version     Show the Docker version information
  wait        Block until one or more containers stop, then print their exit codes
```
7. Display System information using Docker. 
```
Docker system info
```
8. Check whether you can access/download images from DockerHub or not. 
