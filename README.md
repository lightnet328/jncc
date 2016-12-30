# Juniper Network Connect Client
Script for connecting to Juniper VPN through openconnect on macOS(Mac OS X).

Only the ID/PASSWORD connection method is supported.

## Installation
```
$ brew install tuntap
$ brew install openconnect
$ git clone https://github.com/lightnet328/jncc ~/.jncc
$ cp ~/.jncc/jncc.config.example ~/.jncc/jncc.config
$ vim ~/.jncc/jncc.config
$ echo 'export PATH="$PATH:$HOME/jncc"' >> ~/.zshrc
$ exec $SHELL -l
```
If you are using a shell other than zsh please replace `.zshrc` with the appropriate one.

For example, if `/bin/bash` is displayed when `echo $SHELL` is executed, you need to run `echo 'export PATH="$PATH:$HOME/jncc"' >> ~/.bashrc`.

## Connect
```
$ sudo jncc connect
```

## License
MIT License.
See the `LICENSE.txt`.
