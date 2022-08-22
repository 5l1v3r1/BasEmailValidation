# BAS email validation

A simple GUI application for checking email accounts.

# How it works

This application will try to authorize on the provided email accounts via imap/pop3. If authorization is successful and id messages are received - the account will be marked as "good", otherwise it will be marked as "bad".

# Features

## Multithreading

For example, instead of one account, 10 do the same job at the same time. This is much faster, but it is recommended to use only if you have proxies.

## Auto-configuration of the email client

You do not need to search for imap/pop3 settings for your email provider. The application will configure the necessary parameters by itself. Works only for popular domains.
By default, app works on the imap protocol. To work via pop3 go to advanced settings: Settings -> Show Advanced.

## Proxies support

Supported protocols: http, https, socks5.

Uri format: `protocol://username:password@host:port`

Examples:

-   `http://user1:pass1@1.2.3.5:1235`
-   `socks://1.2.3.5:1235`
-   `socks5://user1:pass1@1.2.3.5:1235`
-   `http://127.0.0.1:1235`

# Screens

![tab.accounts](./src-docs/tab.main.png)

# Install

Clone or [download](https://github.com/Sadzurami/BasEmailValidation/archive/refs/heads/main.zip) this repository and run `email.validation.exe`

# Requirements

-   Windows x64 (7+)
-   1 CPU, 512 MB RAM
-   Internet speed 5MB/s +
