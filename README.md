# OpenConnect VPN server

1. Edit [hosts](hosts) file with IP address of instance where to install VPN

2. Adjust [roles/openconnect/defaults/main.yml](roles/openconnect/defaults/main.yml) if needed

3. Generate keys:

```
ssh-keygen
cd ~/.ssh/
cat ~/.ssh/id_rsa.pub >> authorized_keys
chmod 700 ~/.ssh
chmod 600 ~/.ssh/authorized_keys
```

4. Run playbook:
```
ansible-playbook -i hosts playbook.yml
```

5. Use *openvpn* or *Cisco AnyConnect* to connect to VPN server
  
