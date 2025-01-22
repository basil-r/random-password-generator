# Random Password Generator

This repository contains a Node.js script that generates a random password with customizable length. By default, the script generates a 32-character password, but the length can be adjusted by providing a size parameter when running the script.

## Prerequisites

Before using this script, make sure you have the following:

- **Node.js**: The script requires `Node.js` to run. Make sure `Node.js` is installed on your system.

## Installation

Follow these steps to install and set up the script on your system:

1. Clone the repository to your local machine:

```bash
git clone https://github.com/basil-r/random-password-generator.git
cd random-password-generator
```

2. Move the script to a directory in your `PATH` (e.g., `~/bin` or `/usr/local/bin`):

```bash
mv genpass ~/bin/genpass
```

(If `~/bin` doesn't exist, create it with `mkdir ~/bin`.)

3. Make the script executable:

```bash
chmod 700 ~/bin/genpass
```

Now the script is installed and ready to use!

## Usage

To generate a random password, run the script with an optional size parameter:

```bash
genpass 16  # Generates a 16-character password
```

If no size parameter is provided, the script will default to generating a 32-character password:

```bash
genpass  # Generates a 32-character password by default
```

## Example Output

```bash
genpass 16
m@4uB@5CkPz*HxLk
```

## Security Notice

This script generates passwords using the `randomBytes` function from `Node.js's` built-in `crypto` module, which relies on the operating system's cryptographically secure random number generator. While this is generally considered secure for most purposes, always consider additional security measures depending on your use case.

## License

This repository is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.
