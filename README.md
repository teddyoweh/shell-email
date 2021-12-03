# shell-email
 `GET EMAILS DIRECTLY FROM TO TERMINAL TO A TEMPORARY EMAIL `

## Installing Dependencies
- `sudo apt install w3m`
- `sudo apt install curl`
- `sudo apt install jq`

## Usage
```console
$ shell-mail 
-g, --generate [ADDRESS]
        Generate a new email address, either the specified ADDRESS, or
        randomly create one
 
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
