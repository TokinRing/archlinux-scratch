# archlinux-scratch

## Usage

* Build archlinux chroot and import docker image 
```
shmkimage-archlinux.sh
```

### ARM

* The build script on ARM requires the archlinuxarm-keyring to be installed and imported:
```
sudo pacman -S archlinuxarm-keyring
sudo pacman-key --init
sudo pacman-key --populate archlinuxarm
```

**NOTE**: Failing to do the above will result in invalid signature checks on packages installed during the pacstrap phase.
