# printenv.php

A PHP script to output the key-value pairs of a web server's `$_SERVER` environment

## Background

This script was created as a clone of perl script I have seen that do the same. An example can be see at [How to list Perl CGI environment variables](https://alvinalexander.com/perl/edu/articles/pl020001.shtml). The goal is to make it easy see the key-value pairs in this classic, simply way on servers configured for PHP but not Perl. 

The script useful in diagnosing the behavior of PHP applications running on Shibboleth Service Providers among other things.

## Example output

    Shib-Application-ID=urn:org:example:prod:06060
    Shib-Session-ID=_8ea1de51880a532da52505503a5edd33
    Shib-Identity-Provider=https://login.example.org/idp/shibboleth
    Shib-Authentication-Instant=2019-10-31T13:01:26.188Z
    Shib-Authentication-Method=urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport
    Shib-AuthnContext-Class=urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport
    Shib-Session-Index=_2b9a96d6f0cbbef61e34702aa612b3d8
    cn=Pickles,Angelica B
    eppn=apickles@example.org
    givenName=Angelica
    mail=apickles@example.org
    middleName=B
    persistent-id=https://example.org/idp/shibboleth!urn:org:example:prod:06060!1SfTph763MHkmJXJ1FgM/3EY=
    sn=Pickles
    HTTP_HOST=rugrats.example.org
    HTTP_CONNECTION=keep-alive
    HTTP_UPGRADE_INSECURE_REQUESTS=1
    ...
