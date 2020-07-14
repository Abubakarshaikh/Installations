
## Step 1: Update System and Install Required Packages
**Before installing any software, you need to update and upgrade the system you are working on. To do so, run the commands:**
```
sudo apt-get update -y
```
```
sudo apt-get upgrade -y
```

#### Also, make sure to install (or check whether you already have) the following required packages:
```
sudo apt-get install curl
```
```
sudo apt-get install apt-transport-https
```

## Step 2: Install VirtualBox Hypervisor
**1. To install VirtualBox on Ubuntu, run the command:**
```
sudo apt install virtualbox virtualbox-ext-pack
```

#### 2. Confirm the installation with y and hit Enter.
#### 3. Next, the licence agreement appears on the screen. Press Tab and then Enter to continue.
#### 4. The installer asks you to agree with the terms of the VirtualBox PUEL license by selecting Yes.
#### 5. Wait for the installation to complete and then move on to the next step.

### Note: For the VirtualBox hypervisor to work, hardware virtualization must be enabled in your system BIOS.

## Step 3: Install Minikube
#### 1. First, download the latest Minikube binary using the wget command:
```
wget https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```

#### 2. Copy the downloaded file and store it into the /usr/local/bin/minikube directory with:
```
sudo cp minikube-linux-amd64 /usr/local/bin/minikube
```
**There will be no output if the command was executed correctly.**

#### 3. Next, give the file executive permission using the chmod command:
```
sudo chmod 755 /usr/local/bin/minikube
```
**Again, there will be no output.**

#### 4. Finally, verify you have successfully installed Minikube by checking the version of the software:
```
minikube version
```

## Step 4: Install Kubectl
To deploy and manage clusters, you need to install kubectl, the official command line tool for Kubernetes.
#### 1. Download kubectl with the following command:
```
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
```

#### 2. Make the binary executable by typing:
```
chmod +x ./kubectl
```

#### 3. Then, move the binary into your path with the command:
```
sudo mv ./kubectl /usr/local/bin/kubectl
```

#### 4. Verify the installation by checking the version of your kubectl instance:
```
kubectl version -o json
```

## Step 5: Start Minikube
Once you have set up all the required software, you are ready to start Minikube.
#### Run the following command:
```
minikube start
```
#### First, the system downloads the Minikube ISO file from an online source and the localkube binary. Then, it creates a virtual machine in VirtualBox within which it starts and configures a single node cluster.
