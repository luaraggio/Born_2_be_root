<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h1>Born2beRoot</h1>

<h2>Table of Contents</h2>
<ul>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#setup">Setup</a></li>
    <li><a href="#server-configuration">Server Configuration</a></li>
    <li><a href="#strong-password-policy">Strong Password Policy</a></li>
    <li><a href="#sudo-configuration">Sudo Configuration</a></li>
    <li><a href="#monitoring-script">Monitoring Script</a></li>
    <li><a href="#bonus-part">Bonus Part</a></li>
    <li><a href="#conclusion">Conclusion</a></li>
</ul>

<h2 id="introduction">Introduction</h2>
<p>
    This project aims to set up a basic server environment using C, focusing on system administration principles. The server will be configured using a virtual machine (VM) with either Debian or Rocky Linux. This project includes implementing security measures, user management, and monitoring.
</p>

<h2 id="installation">Installation</h2>
<ol>
    <li><strong>Virtual Machine Setup</strong>:
        <ul>
            <li>Use <a href="https://www.virtualbox.org/">VirtualBox</a> or <a href="https://mac.getutm.app/">UTM</a> if VirtualBox is not available.</li>
            <li>Download the latest stable version of Debian or Rocky Linux.</li>
            <li>Create a new VM in VirtualBox/UTM, and ensure to allocate sufficient resources (CPU and RAM).</li>
        </ul>
    </li>
</ol>

<h2 id="setup">Setup</h2>
<p>
    Follow the specific guidelines to set up the server without a graphical interface. Ensure to configure the system to operate in a command-line environment.
</p>

<h2 id="server-configuration">Server Configuration</h2>
<ul>
    <li>Install essential services without a graphical interface (no X.org).</li>
    <li>Set up SSH service on port 4242 and disable root login via SSH.</li>
    <li>Implement a firewall (UFW for Debian or firewalld for Rocky) to allow only port 4242.</li>
</ul>

<h2 id="strong-password-policy">Strong Password Policy</h2>
<p>
    Implement a strong password policy that includes:
</p>
<ul>
    <li>Password expiration every 30 days.</li>
    <li>Minimum of 10 characters, including uppercase, lowercase, and numbers.</li>
    <li>Enforce restrictions on consecutive identical characters.</li>
    <li>Root password must also comply with these rules.</li>
</ul>

<h2 id="sudo-configuration">Sudo Configuration</h2>
<p>
    Configure the sudo access with the following requirements:
</p>
<ul>
    <li>Limit authentication attempts to 3.</li>
    <li>Log all sudo actions, including inputs and outputs.</li>
    <li>Implement TTY mode for security.</li>
</ul>

<h2 id="monitoring-script">Monitoring Script</h2>
<p>
    Create a bash script named <code>monitoring.sh</code> to display system information every 10 minutes, including:
</p>
<ul>
    <li>Architecture and kernel version.</li>
    <li>Number of physical and virtual processors.</li>
    <li>RAM and storage utilization.</li>
    <li>Current CPU load and active connections.</li>
    <li>IP address and MAC address of the server.</li>
</ul>

<h2 id="bonus-part">Bonus Part</h2>
<p>
    For bonus points, consider implementing additional features, such as:
</p>
<ul>
    <li>Setting up functional WordPress services.</li>
    <li>Choosing an additional service to install and justify its utility.</li>
</ul>

<h2 id="conclusion">Conclusion</h2>
<p>
    The Born2beRoot project emphasizes the importance of understanding system administration, security measures, and proper server configuration. Ensure that all requirements are met and the server operates smoothly for a successful defense.
</p>

</body>
</html>
