# README

## Overview

This repository provides scripts to generate and verify signatures using SSH keys.

## Prerequisites

- Ensure you have `ssh-keygen` installed.
- Ensure you have a valid SSH key pair.

## Usage

### Generate a Signature

To generate a signature for a message, use the `generate` script.

    bash <(curl -sL https://caoer.github.io/sign/generate)

If you do not provide a message as an argument, the script will prompt you to enter one.

### Verify a Signature

To verify a signature, use the `verify` script.

    bash <(curl -sL https://caoer.github.io/sign/verify)

The script will prompt you to enter the message, GitHub username, and the signature. The signature can be multiline; press Enter on a blank line to finish inputting the signature.

## Example

### Generating a Signature

./generate "Hello, World!"

### Verifying a Signature

./verify

You will be prompted to enter the message, GitHub username, and the signature.

## License

This project is licensed under the MIT License.
