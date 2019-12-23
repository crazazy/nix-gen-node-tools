# nix-js-tools

this tool generates node.js command line tools that were written in pure javascript

it uses [node2nix](https://github.com/svanderburg/node2nix) to generate the necessary nix expressions to fetch them

other than that, this application requires `jq` and `curl` to function

## Usage:

to get nix expressions for your CLI tool of choice type './standalone {npm package name}', and put the resulting folder in your package set.

Alternatively you can check out a installable version at my [personal repository](https://github.com/crazazy/nixos-config) so that you can create these folders anywhere on your computer

You can test out the contents immediately by going into the resulting folder and typing `nix-build -A package`, then going to result/bin/{program name}
