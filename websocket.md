# Websocket Cheat Sheet

A cheat sheet for Websocket commands.

#

[variable] = placeholder for a variable

#

### curl to a websocket server

> curl -i -N -H "Connection: Upgrade" -H "Upgrade: websocket" -H "Host: localhost:8080" -H "Origin: http://localhost:8080" http://localhost:8080
