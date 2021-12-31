# directory2apt
Make any folder an APT repository

# Installing

```bash
sudo wget "https://raw.githubusercontent.com/sudo-give-me-coffee/directory2apt/main/directory2apt" -O "/usr/bin/directory2apt"
sudo chmod a+x "/usr/bin/directory2apt"
```

# Uninstalling

```bash
sudo rm "/usr/bin/directory2apt"
```

# How to use

This only requires 2 steps:

#### 1. Create directory and put the Debian packages files inside it
In this step all you need to do is create a folder and place the .deb files inside it.

#### 2. Run `directory2apt`

In this step you call the `directory2apt` passing the directory created on step 1, for e.g.:

```
sudo directory2apt /var/custom-apt-repo
```

> Note that the directory will be owned by root at the end of step

# Disabling the custom repo

Just remome the source related file in `/etc/apt/sources.list.d`
