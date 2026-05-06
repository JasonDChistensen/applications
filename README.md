# applications
Applications to install

# Update the package repositories
sudo apt update

# IDE's
visual studio code

# CUDA
sudo apt install nvidia-cuda-toolkit

# Mastering embedded Linux Development
sudo apt-get install autoconf automake bison bzip2 cmake flex g++ gawk gcc gettext git gperf help2man libncurses5-dev libstdc++6 libtool libtool-bin make patch python3-dev rsync texinfo unzip wget xz-utils

sudo apt-get install arp-scan

sudo apt-get install autoconf e2fsprogs genext2fs mtd-utils squashfs-tools util-linux

sudo apt install python3-venv

sudo apt install smem

sudo apt  install valgrind

# Buildroot
https://buildroot.org/downloads/manual/manual.html#requirement

## Mandatory packages
sudo apt-get install autoconf which sed make binutils build-essential diffutils gcc g++ bash patch gzip bzip2 perl tar cpio unzip rsync file bc findutils awk gawk wget

## buildroot Optional packages
sudo apt-get install autoconf python ncurses5 qt5 glib2 gtk2 glade2
sudo apt-get install autoconf bzr curl cvs git mercurial openssh-client subversion
sudo apt-get install autoconf default-jdk default-jre asciidoc w3m python3 dblatex graphviz python3-matplotlib python3-aiohttp

# Other
sudo apt install tmux


# Docker
1. Update the package repositories:
$ sudo apt update
2. Install Docker:
$ sudo apt install docker.io
3. Start the Docker daemon and enable it to start at boot time:
$ sudo systemctl enable --now docker
4. Add yourself to the docker group:
$ sudo usermod -aG docker <username>
5. Restart the Docker daemon:
$ sudo systemctl restart docker

To see a list of Docker images:
```
$ docker images
```

To build a image:

-t, --tag stringArray               Image identifier (format: "[registry/]repository[:tag]")

```
$ docker build -t my-image .
```

To run the image
```
docker run: Tells Docker to create and start a new container from a specific image.
-i (interactive): Keeps the "Standard Input" (STDIN) open even if not attached. This allows you to
   send commands to the container.
-t (tty): Allocates a virtual terminal (pseudo-TTY) inside the container. This makes the interface
   look and behave like a real terminal session (e.g., providing a command prompt like root@containerID:/#).
--mount type=bind,source=/host/path,target=/container/path,readonly
-w Setting the Working Directory: If you want the container to start inside the directory you just
   mounted, use the -w or --workdir flag
```
  
$ docker run -it --mount type=bind,source=/home/jason,target=/home/jason -w /home/jason my-image

To exit, type: exit








