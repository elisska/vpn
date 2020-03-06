# OpenConnect VPN server

1. Edit [hosts](hosts) file with IP address of instance where to install VPN

2. Adjust [roles/openconnect/defaults/main.yml](roles/openconnect/defaults/main.yml) if needed

3. Run playbook:
```
ansible-playbook -i hosts playbook.yml
```

4. Use *openvpn* or *Cisco AnyConnect* to connect to VPN server
  
