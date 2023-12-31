# Open-Roaming-Byzn (ORB)
ORB is a command-line script that connects to the OpenAI API to harness the power of ChatGPT models for generating human-like text responses. It's designed to provide a seamless interface for interacting with OpenAI's language models.

## UPDATE 10/15/2023
- Created separate `install.sh` for smoother install.
- Modified she-bang statements from FreeBSD's `/usr/local/bin/zsh` to Linux `/usr/bin/zsh`
- Install.sh will now check for both `jq` and `zsh` and install if neccessary.
- Install.sh will now check if user uses `doas` or `sudo`. The script checks first for `doas` since it is not so common.


## Features
### Secure API Key Input: 
ORB allows you to securely input your OpenAI API key without displaying it on the screen.

### Easy Installation: 
It checks if the essential JSON processing tool `jq` is installed and if `zsh` is installed, and installs them if necessary, ensuring a smooth setup process.

### Chat with ChatGPT: 
With ORB, you can engage in a conversation with the ChatGPT model using the "babbage" model ID. It's a versatile tool for various text generation tasks.

### Exit Gracefully: 
ORB is user-friendly and lets you exit the conversation by typing 'exit.'

## Usage
Ensure you have the OpenAI API key ready.

Run the script.

Input your conversation prompts, and receive responses from ChatGPT.

Type 'exit' to gracefully end the conversation.

## Requirements
Zsh shell  
jq (a JSON processor)

## Installation -- Debian GNU/Linux

1. Clone this repository
2. unzip orb-main.zip
3. `cd` to orb-main
4. `chmod +x` install.sh
5. run `./install.sh`

## Installation -- FreeBSD

1. Clone this repository
2. unzip orb-main.zip
3. `cd` to orb-main
4. Modify `orb` she-bang to `#!/usr/local/bin/zsh`
5. `chmod +x` install.sh
6. run `./install.sh`

## How to Get an OpenAI API Key
To use this script, you need an OpenAI API key. You can obtain one by signing up for an account on the OpenAI platform.

**Disclaimer**  
This script is intended for educational and testing purposes. Ensure you comply with OpenAI's usage policies and respect rate limits when using the OpenAI API.
