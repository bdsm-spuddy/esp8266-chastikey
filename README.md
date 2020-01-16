# esp8266-chastikey
Example of how to talk to the chastikey API and decode the JSON API

I split out the defines for network connectivity to a separate file so
that this file can be added to .gitignore.  It means I can publish my
sketches to git without exposing passwords.

Basically just create a `network_conn.h` with the two following lines:

    const char* ssid       = "YOURSSID";
    const char* password   = "YOURPSWD";

The `Makefile` is for command line users using `arduino-cli`
