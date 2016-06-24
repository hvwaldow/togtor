# togtor

## Description

A shell script that toggles [Tor](https://www.torproject.org/) on or
off.  It checks for a running [Privoxy](https://www.privoxy.org/),
starts the onion-proxy, if necessary, patches the Privoxy config file,
checks for success and prints the new IP address.

## Usage

    togtor
    togtor on | off
    togtor -h

The first form gives status information.<br />
The second form switches tor mode on or off.<br />
The third form displays usage instructions.<br />

## Assumptions

+ We assume Privoxy is installed and running.
+ We assume the Privoxy config is in /etc/privoxy/config.
+ The executing user can sudo (passwordless preferred).
+ This is a systemd - system.

## Notes

+ To browse the web using Tor/Privoxy, you have to set the proxy setting of your browser accordingly.
+ Consider using the [browserbundle](https://www.torproject.org/projects/torbrowser.html.en).
+ You are most likely not anywhere anonymous unless you studied enough
  of the
  [documentation of the Tor Project](https://www.torproject.org/docs/documentation.html.en).
