# Logs

Logs is a BurpSuite extension to work with log files.

With this simple extension you will be able to load Burp's log files into Burp, and perfom actions like sending a specific request to the Repeater to perform further attacks or analysis.

Under Project Options > Misc > Logging, there are options to log every HTTP request and response made and received by Burp. Logging can be configured per-tool or for all Burp traffic. This can be useful to keep __complete__ records of your sessions.


## Features
- A tab within the main Burp UI.
- A log table and two instances of Burp's own HTTP message editor, which display the selected request and response (as in the Proxy history).
- Right-clicking the message editor produces the classic Burp's context menu used to perform actions like sending the message to other Burp tools, request/show in browser, copy as curl command, etc.


## Building instructions
- Clone the repo.
- Make a couple of dirs: `mkdir bin build`
- Build the Logs jar: `javac -d build/ src/burp/*.java; jar cf bin/Logs.jar -C build/ burp`
- Load your `bin/Logs.jar` into Burp.

