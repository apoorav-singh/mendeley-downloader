# Mendeley API Python Downloader #

## Functionality

Unfortunatly there is no Bulk download feature in Mendeley as of now and you may not access the PDFs in your local storage.
This project is a workaround to download all files in your Library at once. Very basic.

## How to run

Project is based on https://github.com/Mendeley/mendeley-api-python-example.git

Register an app at https://dev.mendeley.com/ use `http://127.0.0.1:5000/oauth` as redirect URL

1. Create a `config.yml` by copying the example file and insterting cliend id/secret of your app
2. Run the python file after the installation of the requirements.
3. Visit `http://127.0.0.1:5000/oauth`

Use Python 3.8 or older, otherwise you will encounter issues with the mendeley SDK

## Changes

1. The original URL `http://localhost:5000` won't work as the solution is suggested at `https://github.com/Mendeley/mendeley-api-python-example/issues/3#issuecomment-207752071`.
2. Remove curly braces from the config.yml file. Example:
3.   clientId: {YourID} to clientId: 00000
