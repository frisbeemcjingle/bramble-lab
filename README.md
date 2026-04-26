# bramble-lab
## Recovering from IP change
If k3s crashes after a network change, update /etc/rancher/k3s/config.yaml:
  node-ip: <current-wifi-ip>
  flannel-iface: wlan0
  disable-network-policy: true
Then: sudo systemctl restart k3s
