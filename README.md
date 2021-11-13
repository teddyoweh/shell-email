# terminal-email
 `tmpmail` is a command line utility written in POSIX `sh` that allows you to create a temporary email address and receive emails to the temporary email address. It uses 1secmail's [API](https://www.1secmail.com/api/) to receive emails.

## Installing Dependencies
- `sudo apt install w3m`
- `sudo apt install curl`
- `sudo apt install jq`

## Usage
```console
$ tmpmail --help
tmpmail
tmpmail -h | --version
tmpmail -g [ADDRESS]
tmpmail [-t | -b BROWSER] -r | ID

When called with no option and no argument, tmpmail lists the messages in
the inbox and their numeric IDs.  When called with one argument, tmpmail
shows the email message with specified ID.

-b, --browser BROWSER
        Specify BROWSER (default: w3m) that is used to render the HTML of
        the email
-g, --generate [ADDRESS]
        Generate a new email address, either the specified ADDRESS, or
        randomly create one
-h, --help
        Show help
-r, --recent
        View the most recent email message
-t, --text
        View the email as raw text, where all the HTML tags are removed.
        Without this option, HTML is used.
--version
        Show version
```

### Examples
Create random email
```console
$ tmpmail --generate
xoithrjagpx@1secmail.net
```
