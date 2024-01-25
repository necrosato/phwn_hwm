# pwn_hwm

define networks which your pwnagotchi will attempt to establish a connection to,
displaying the ip address to easily connect to your pwnagotchi without a usb connection.

You can define multiple networks, just ensure that networks is alternating ssid/password.
Unfortunately, pwnagotchi loader cannot handle maps or lists of lists, and toml doesn't
support keys with spaces.
```
main.plugins.pwn_hwm.enabled = true
main.plugins.pwn_hwm.networks = [
    'your_home_network_ssid', 'your_home_network_password',
    'Your network with spaces', 'a password with spaces'
]
main.plugins.pwn_hwm.minimum_rssi = -75
```
