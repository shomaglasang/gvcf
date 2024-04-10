# OpenVPN Configuration Generator (gvcf)
OpenVPN configuration file (.ovpn) generator for devices and users. The script is written for environments with an OpenVPN server and multiple devices and users.
1. Generate .ovpn configuration for devices.
2. Generate .ovpn configuration for users (allows users to access devices over VPN).
3. Auto-calculate and assign VPN IP address.
4. Command-line inputs/parameters.
5. Write meta-data to DB (mysql) for UI integration.
6. Upload and apply .ovpn configuration file into device.
7. Bulk generation.
8. Check expired or expiring .ovpn configuration file.


# Usage
--
Generate device config:
```
gvcf.php -c "MY VPN CA" -n "device-1" -d 10.10.0 -v
```

Generate and install config into the device:
```
gvcf.php -c "MY VPN CA" -n "device-2" -d 10.10.0 -v -V -S -D -U -R -I 123.123.123.123 -P 22 -X PASSWORD
```

