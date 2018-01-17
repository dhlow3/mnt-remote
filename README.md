# mnt-remote

> Helper script to mount and unmount a drive over a network.

## Tested On
Ubuntu 16.04.2 LTS

## Requirements
* sshfs: a filesystem client based on ssh
* fusermount: unmount FUSE filesystems

## Setup
1. mkdir ~/remote on client
2. put mnt-remote somewhere like ~/bin or other directory listed in $PATH
3. sudo chmod 755 mnt-remote

## Usage
1. determine the user and host address on the remote computer
2. type mnt-remote user@hostaddress to mount drive on remote computer
3. type mnt-remote -u to unmount drive

## Notes
* script assumes there is a ~/remote directory on the client computer
 * change script if you'd rather the mount point be in a different directory
* script assumes the entry point on the remote drive will be /home/user
