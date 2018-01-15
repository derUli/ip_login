# ip_login

Login users based on their ip address.

## Disclaimer

All IP addresses in this document were randomly generated. 
The UliCMS project is not associated in any form with the owners of these addresses.

Words included in brackets in this document are intended as placeholders. 

**Example:** 

```
[IP Address]
```

## What is ip_login?

ip_login is an UliCMS module for logging in Users based on their ip address. When a client with the IP address [ip address] accesses your UliCMS backend [user name] will automatically get logged in without the need to fill the login form. If a user is authenticated by his ip address the logout button is disabled, since it won't work in this case.
If the IP address of a ip authenticated user changes he will get logged out.

ip_login will coexist with other authentication modules and methods.

## Requirements

* UliCMS 2018.2 or a later version of UliCMS 2018.x

## Configuration

To configure IP-to-User Mappings your usergroup needs the permission **ip_login**.


1. Click **Packages** > **ip_login** > **Settings**
2. There is a textarea for mapping ip addresses to a user.

One entry per line
The format must be:

```
[IP Address]=>[Username]
```

Here are some example mappings:

```
131.213.138.20=>maxmuster
209.143.210.186=>sabinemuster
60.226.125.233=>johndoe
```