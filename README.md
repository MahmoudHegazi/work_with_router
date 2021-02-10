# work_with_router
https://hub.packtpub.com/using-python-automation-to-interact-with-network-devices-tutorial/  

### step1
```
pip install netmiko
```

### step2

```
from netmiko import ConnectHandler
# device_type can got from router page
device = ConnectHandler(device_type=’cisco_ios’, ip=’192.168.255.249′, username=’cisco’, password=’cisco’)
output = device.send_command(“show version”)
print (output)
device.disconnect()


```
