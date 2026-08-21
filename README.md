#  OverTheWire: Bandit (Level 20+) - Walkthrough & Security Notes

This repository contains my technical notes, commands, and logic while solving levels 20 through 34 of the [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) wargame.

> **Note:** Levels 0–19 were completed prior to establishing this public documentation log. Focus in this repository is placed on intermediate/advanced Linux security concepts (Level 20+).

### **Level 20 - 21**
**OBJECTIVE:-**  Make a connection with the setuid binary through any localhost port and pass the password of the current level

**KEY COMMAND:-** `echo "password" | nc -l -p <port> &`
 
**Concept:-** Create a backgroud listening port using Netcat (`nc -l`) followed by (`&`) which makes it run in the background and then just pass the port to the setuid binary using (`./suconnect <post>`) so that it could establish the connection and verify the password.