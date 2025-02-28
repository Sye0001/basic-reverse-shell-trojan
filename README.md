# basic-reverse-shell

<h1>script is a basic reverse shell that connects to a remote command-and-control (C&C) server. Here's a summary of its functionality:</h1>

<h2>1</h2> Autorun: <p>The script attempts to copy itself to the Windows Startup folder to ensure it runs automatically on system boot.</p>

<h2>2</h2> Connection:<p> It establishes a connection to a remote server specified by CCIP (IP address) and CCPORT (port).</p>

<h2>3</h2> Command Execution: <p>Once connected, it listens for commands from the server, executes them on the victim's machine using subprocess, and sends the output back to the server.</p>

<h2>4</h2> Persistence: <p>If the connection is lost, it continuously attempts to reconnect every 3 seconds.</p>
