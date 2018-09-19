# cmdline-cast

This component casts the command line to a server to help students at my lectures in Linux at the [University for Applied Sciences FH Burgenland](http://www.fh-burgenland.at/). Burgenland is a federal state of Austria, the name would translate to castles country.

## How it works

The last command line is captured by setting `PS0` in the Bash environment. Bash version must be >= 4.4 for this feature.

This command line is then sent via a REST API to a server implemented in [Meteor](https://www.meteor.com/). The server is available at https://github.com/fknipp/cmdline-server.

## Installation

1. Clone this repository.
1. Create a symbolic link from `cmdline-cast` to `/usr/local/bin`.
1. Execute `cmdline-cast login` and enter your credentials.
1. Execute `cmdline-cast start` in your current shell:

    ```
    . cmdline-cast start
    ```
    This sets the necessary environment variables to log all commands to the server. This might be part of `/etc/bash.bashrc` or `~/.bashrc`.
1. Enjoy seeing your commands on https://cmdline.qnipp.com.

## Status

This in work in progress. I've many more features in mind to make it easier for my students to follow the lectures.


## License

MIT