# 💻 Basic Reverse Shell

<div style="background-color: #fff3cd; padding: 10px; border: 1px solid #ffeeba; border-radius: 5px; margin: 10px 0;">
    <h3 style="color: #856404; margin: 0;">⚠️ SOFTWARE IS POSSIBLY OUTDATED | USE AT YOUR OWN RISK</h3>
</div>

<p style="text-align: center; text-decoration: underline;">The script is a basic reverse shell that connects to a remote command-and-control (C&C) server. Here's a summary of its functionality:</p>

<div style="display: flex; align-items: baseline;">
    <h4 style="margin: 0 10px 0 0;">1.</h4>
    <p><strong>Autorun:</strong> The script attempts to copy itself to the Windows Startup folder to ensure it runs automatically on system boot.</p>
</div>

<div style="display: flex; align-items: baseline;">
    <h4 style="margin: 0 10px 0 0;">2.</h4>
    <p><strong>Connection:</strong> It establishes a connection to a remote server specified by <code>CCIP</code> (IP address) and <code>CCPORT</code> (port).</p>
</div>

<div style="display: flex; align-items: baseline;">
    <h4 style="margin: 0 10px 0 0;">3.</h4>
    <p><strong>Command Execution:</strong> Once connected, it listens for commands from the server, executes them on the victim's machine using <code>subprocess</code>, and sends the output back to the server.</p>
</div>

<div style="display: flex; align-items: baseline;">
    <h4 style="margin: 0 10px 0 0;">4.</h4>
    <p><strong>Persistence:</strong> If the connection is lost, it continuously attempts to reconnect every 3 seconds.</p>
</div>
