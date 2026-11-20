# Flowrensic for Cadence CLI

Flowrensic runs beside your durable workflow engine and finds problems in your workflows. Flowrensic for Cadence finds problems in Cadence workflows. Its server has 20 finding classes ported from Temporal and one of its own, Activity retrying, and a findings page with filters for severity, class, domain, workflow type and status.

This is the command line client, cadence-flowrensic, for your CI. It asks a Flowrensic for Cadence server how it is.

Each release puts the binaries here, for Linux amd64, Linux arm64 and macOS arm64, with checksums.txt. This repo is written by the release and is not edited by hand.

Quickstart: https://cadence.flowrensic.com/docs/quickstart/

## Install

For Linux on arm64 or a Mac, change linux-amd64 to linux-arm64 or darwin-arm64:

    curl -fsSL -o cadence-flowrensic https://github.com/flowrensic/cadence-flowrensic-cli/releases/latest/download/cadence-flowrensic-linux-amd64
    chmod +x cadence-flowrensic

Check the binary against checksums.txt on the same release page.

## Use

    ./cadence-flowrensic status http://localhost:8080

It prints the health, the version and the number of findings of the server, and ends with 1 when the server is not healthy. Without a URL it asks http://localhost:8080.

    ./cadence-flowrensic version

prints the version of the CLI.

## Learn more

- Quickstart: https://cadence.flowrensic.com/docs/quickstart/
- Packages: https://cadence.flowrensic.com/docs/packages/
