### Wireguard vpn server for Kubernetes/k8s

Hey there. 
This is very minimalist snippet which allows to run wireguard vpn server pod in k8s single node cluster. 

Before applying manifest to k8s don't forget to change `<server_public_port>` to corresponding value.

If you have multi node environment make sure you are running wireguard pod at [specific node](https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/).

After first start directory `/wg-config` will be created at parent node. It will contain peers configurations in order to use VPN. Both QR codes and `.conf` files.
