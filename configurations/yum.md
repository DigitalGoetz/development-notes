# Yellowdog Update Manager (yum)

Instructions sourced from [here](https://stackoverflow.com/questions/36651091/how-to-install-packages-in-linux-centos-without-root-user-with-automatic-depen)

## Configure for low-privilege environments

```bash
mkdir ~/centos

export PATH="$HOME/centos/usr/sbin:$HOME/centos/usr/bin:$HOME/centos/bin:$PATH"
export MANPATH="$HOME/centos/usr/share/man:$MANPATH"

L='/lib:/lib64:/usr/lib:/usr/lib64'
export LD_LIBRARY_PATH="$HOME/centos/usr/lib:$HOME/centos/usr/lib64:$L"
```

## Find Packages

```bash
yum search 
mkdir ~/rpm
```

### Install RPMS

```bash
cd ~/centos && rpm2cpio ~/rpm/x.rpm | cpio -id
```
