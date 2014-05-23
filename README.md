#SFTP-Deployment for Atom.io

Spend less time managing file transfers and more time coding. SFTP support for Atom.io to send and receive files directly in your server.

SFTP-Deployment is a package for Atom.io using [SSH2 client](https://github.com/mscdex/ssh2) module written in pure Javascript for [node.js](http://nodejs.org/).

![SFTP-deployment](https://atom.io/assets/packages-d6c259ff67b995961012620be1e26678.gif "SFTP-deployment")


##Features

###Workflows
* Working off of a server
  * Create, edit, rename and delete files
  * Create, rename and delete folders
* Upload files
* Download files

###Compatibility
* Supports SFTP servers
* Works on Windows, OS X and Linux

###Integration
* menu entries and command palette control
* File-based configuration (JSON)
* Colorized output panel with options for automatic hiding

## Installation

1. Search `sftp` in the atom package manager
2. Since the installation is successful, you can generate the configuration file with the command
  * `cmd-shift-p` and search `mapToRemote`
  * Packages menu -> SFTP -> Map to Remote...
  * Create your own
3. Set your sftp configuration in this file
4. Use it!

####Example of configuration file:
```
{
  "host": "127.0.0.1",
  "username": "identifier",
  "password": "secret_password",
  "port": "22",
  "destDir": "/home/myuser/project/path"
}
```

##Next Versions

###Workflows
* Working off of a server
  * Create, edit, rename and delete files
  * Create, rename and delete folders
* Upload folders, or just the changes since your last commit
* Download folders

###Compatibility
* Supports FTP, FTPS servers
* Supports both implicit (port 990) and explicit SSL for FTPS connections
* Password and SSH key auth with SSH agent support
* Detects and informs about SSH host key changes
* Can detect changes via Git, Mercurial and SVN

###Integration
* Keyboard shortcuts
* Secure password and passphrase entry

##Version
* `0.0.1` Build the first atom package
