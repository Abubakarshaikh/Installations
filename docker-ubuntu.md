# Install Docker From a standard Ubuntu Repository

## Step 01: Use the apt command to install the docker.io package:
```
 $ sudo apt install docker.io
```

## Step 02: Start docker and enable it to start after the system reboot:
```
$ sudo systemctl enable --now docker
```

## Step 03: Optionally give any user administrative privileges to docker:
```
$ sudo usermod -aG docker SOMEUSERNAME
```

## Step 04: Check docker version:
```
$ docker --version
```

## Step 05: Run docker test using the hello-world container:
```
$ docker run hello-world
```
