# cmdline-cast

Cast the command line to a server to help students at the lectures.

## How it works

The last command line is captured by setting `PS0` in the Bash environment. Bash version must be >= 4.4 for this feature.

This command line is then sent via a REST API to a server implemented in Meteor.

## License

MIT