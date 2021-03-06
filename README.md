Virtualhost Manage Script
===========

Bash Script to allow create or delete apache virtual hosts on Ubuntu in a quick way.

## Installation ##

1. Download the script
2. Apply permission to execute:

```
$ chmod +x /path/to/virtualhost.sh
```

3. Optional: if you want to use the script globally, then you need to copy the file to your /usr/local/bin directory, is better
if you copy it without the .sh extension:

```bash
$ sudo cp /path/to/virtualhost.sh /usr/local/bin/virtualhost
```

### For Global Shortcut ###

```bash
$ cd /usr/local/bin
$ wget -O virtualhost https://raw.githubusercontent.com/anilnautiyal/virtualhost/master/virtualhost.sh
$ chmod +x virtualhost
```

## Usage ##

Basic command line syntax:

```bash
$ sudo sh /path/to/virtualhost.sh [create | delete] [domain] [optional host_dir]
```

With script installed on /usr/local/bin

```bash
$ sudo virtualhost [create | delete] [domain] [optional host_dir]
```

### Examples ###

to create a new virtual host:

```bash
$ sudo virtualhost create project.dev
```
to create a new virtual host with custom directory name:

```bash
$ sudo virtualhost create project.dev full_dir
```
to delete a virtual host

```bash
$ sudo virtualhost delete project.dev
```

to delete a virtual host with custom directory name:

```
$ sudo virtualhost delete project.dev full_dir
```

Forked From [RoverWire/virtualhost](https://github.com/RoverWire/virtualhost)
