**Upgrading Package Database**
```
$ sudo apt-get update
```


**It looks like you’re running macOS, Linux, or another Unix-like OS. To download Rustup and install Rust, run the following in your terminal, then follow the on-screen instructions.**
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
OR
```
sudo apt install rustc
```


**You can uninstall at any time and these changes will be reverted.**
```
with rustup self uninstall
```

**Now you can verify the version of Rust installed in your Ubuntu.**
```
rustc --version
```

**Install Build Tools for Rust, Rust program needs to be complied before running the file. So you need to install build-essentials**
```
sudo apt install build-essential
```
