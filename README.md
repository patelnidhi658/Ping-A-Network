Ping Host
This is a simple Python script that allows you to ping a host using the ping command on Unix-based systems. The script uses the subprocess module to execute the ping command and returns the output as a string.

Installation:
No installation is required to use this script. You just need to have Python 3 installed on your system.

Usage:
To use this script, simply call the 'ping' function and pass the host you want to ping as an argument. 
For example:
import subprocess

def ping(host):
    result = subprocess.run(['ping', '-c', '3', host], stdout=subprocess.PIPE)
    return result.stdout.decode()

print(ping('google.com'))

This will ping 'google.com' three times and return the output as a string.
