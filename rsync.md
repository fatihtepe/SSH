From Wikipedia:

rsync is a software application for Unix and Windows systems which synchronizes files and directories from one location to another while minimizing data transfer using delta encoding when appropriate. An important feature of rsync not found in most similar programs/protocols is that the mirroring takes place with only one transmission in each direction. rsync can copy or display directory contents and copy files, optionally using compression and recursion.

In daemon mode, rsync listens on the default TCP port of 873, serving files in the native rsync protocol or via a remote shell such as RSH or SSH. In the latter case, the rsync client executable must be installed on both the local and the remote host.

- progress: will show the percentage of the file copied
- partial: tells rsync to keep the partial file which should make a subsequent transfer of the rest of the file much faster.
- a: Archive, It is a quick way of saying you want recursion and want to preserve almost everything.
- v: Verbose
- z: Compress the files so less bandwidth is needed, and the files are copied faster.

## Synchronize two folders with rsync

If you want to keep two folders in sync rsync is also your best option.

*From local to remote computer

rsync -av --delete /source/folder user@remote.server:/destination/folder

*From remote to local computer

rsync -avz --delete user@remote.server:/source/folder /destination/folder

* The --delete option will delete the files in the destination folder, that have been deleted in the source folder, that way the two folders will always be in sync.

<a href="https://www.garron.me/en/go2linux/rsync-backup-linux-using-rsync-to-backup-files-or-folder-under-linux.html">source</a>
