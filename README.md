phing-stuff
===========

Assorted phing stuff


### FileRsyncTask

Keep in sync 2 file-trees using rsync.

#### Example

    <rsync
      rsyncPath="${rsync.executable}"
      sourcedir="${rsync.source}"
      destinationdir="${rsync.dest}"
      delete="${rsync.delete}"
      excludefile="${rsync.excludefrom}"
      filesfromfile="${rsync.filelist}"
      backupdir="${rsync.backupdir}"
      checksum="${rsync.usechecksum}"
      identityfile="${rsync.sshkey}"
      remoteshell="${rsync.remoteshell}"
      dryrun="${rsync.testonly}"
      verbose="${rsync.debug}"
      itemizechanges="${rsync.showchanges}"
      options="${rsync.option}" />

Either `sourcedir` or `destinationdir` can be in the form `<user>@<host>:/path/to/dir`

Latest update introduces `filesFromFile` option to selectively upload files
