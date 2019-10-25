# Project Development

For general information about contributing changes, see the
[Contributor Guidelines](https://github.com/titan-data/.github/blob/master/CONTRIBUTING.md).

## How it Works

Take the dockerized SSH service and add some additional commands we need for
titan.

## Building

Builds are done with `docker build`.

## Testing

To test the image, build it locally and tag it as
`titandata/ssh-test-server:latest`. Run the `titan-server` end to end tests and
ensure that they work.

## Releasing

Given how infrequently we expect this to be updated (if ever), we simply build
a new `latest` tag with every push through DockerHub's built-in build
processes.
