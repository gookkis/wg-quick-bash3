# What is Wireguard ?
WireGuard® is an extremely simple yet fast and modern VPN that utilizes state-of-the-art cryptography. It aims to be faster, simpler, leaner, and more useful than IPsec, while avoiding the massive headache. It intends to be considerably more performant than OpenVPN. WireGuard is designed as a general purpose VPN for running on embedded interfaces and super computers alike, fit for many different circumstances. Initially released for the Linux kernel, it is now cross-platform (Windows, macOS, BSD, iOS, Android) and widely deployable. It is currently under heavy development, but already it might be regarded as the most secure, easiest to use, and simplest VPN solution in the industry.

# What is wg-quick ?
`wg-quick` is a script that helps you easily set up a WireGuard VPN interface. It can read an existing configuration file and apply the settings therein to a VPN interface. When you're done, it can tear down the interface and clean up after itself.

# Why wg-quick-bash3 ?
`wg-quick` is written in bash and it uses some bash features that are not available in bash version 3.xx which is officially bundled with MacOS. This script is a workaround to make `wg-quick` works on MacOS.

# How to use ?
1. Download the script
2. Make it executable
3. Run it with `sudo` or as `root`
4. Use `wg-quick` as usual
5. Enjoy

# Example
```bash
$ sudo ./wg-quick-bash3 up wg0
[#] ip link add wg0 type wireguard
[#] wg setconf wg0 /dev/fd/63
[#] ip -4 address add
```

# Give Star if you like it
If you like this script, please give it a star. It will help me to improve the script.

# License
This script is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

