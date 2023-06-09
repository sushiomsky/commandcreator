# ChatGPT Command/Script Generator

This script takes a string as an argument and sends it to the ChatGPT API to generate a command or a script. The generated command or script is printed to stdout. If no string is given as an argument, the user is prompted to enter one. The OpenAI API key is retrieved from the shell variable $OPENAI_API_KEY or the user is prompted to enter it if not present. The entered API key is stored for future use.

## Usage

1. Ensure you have Python 3 installed.
2. Install the required dependencies by running the following command:
    ```
    pip install openai
    ```
3. Set the `OPENAI_API_KEY` environment variable with your OpenAI API key.
4. Run the script with the desired string as an argument:
    ```
    python script.py "Your input string"
    ```
   Alternatively, you can run the script without any arguments and enter the string when prompted.

## API Key

The script retrieves the OpenAI API key from the `OPENAI_API_KEY` environment variable. If the variable is not set or the API key is invalid, the script will prompt you to enter the API key.

## Supported Shells

The script supports the following shells: `zsh`, `bash`, and `sh`. If your current shell is one of these, it will be used for generating the command or script. Otherwise, `bash` is used as the default.

## Generated Command

To generate a command, provide a string as an argument. The script will use the ChatGPT API to generate a command based on the input string and print it to stdout.

Example:
python script.py "Create a new directory"

## Generated Script

To generate a script, use the `-s` option followed by the string. The script will use the ChatGPT API to generate a script based on the input string and print it to stdout. You will also be prompted to provide a filename for the script.

Example:
python script.py -s "Install dependencies"


## License

This script is licensed under the GPL-3.0 license.

## Author

Dennis Kelly Suchomsky

## Date

June 2023
