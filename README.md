## Overview

PKI setup for Mongo Server certificates

## Setup

Use the `init-pki` command to created the directory structure

Then create a certificate request 

```
easyrsa gen-req mongoserver

Using SSL: openssl OpenSSL 1.1.0g  2 Nov 2017
Generating a 2048 bit RSA private key
..+++
...............................................................................+++
writing new private key to '/home/fiona/wd/dwp/cis/enterprise_mongo_server/pki/private/mongoserver.key.lfNnD8JYZx'
Enter PEM pass phrase:
Verifying - Enter PEM pass phrase:
-----
You are about to be asked to enter information that will be incorporated
into your certificate request.
What you are about to enter is what is called a Distinguished Name or a DN.
There are quite a few fields but you can leave some blank
For some fields there will be a default value,
If you enter '.', the field will be left blank.
-----
Common Name (eg: your user, host, or server name) [mongoserver]:

Keypair and certificate request completed. Your files are:
req: /home/fiona/wd/dwp/cis/enterprise_mongo_server/pki/reqs/mongoserver.req
key: /home/fiona/wd/dwp/cis/enterprise_mongo_server/pki/private/mongoserver.key

``` 
