# Configuration Options

### Notes: 
* If you enable Ingress/Reverse Proxy for Handbrake, you need to have `SECURE_CONNECTION`=0 and Port Type set to `HTTP`, otherwise you may run into errors for `Too many redirects`.
* VNC can't be Ingressed/Reversed Proxied. if you want to use VNC, you must set this service to `NodePort` instead of `clusterIP`.
* VNC with `SECURE_CONNECTION`=1, only works with very few clients. One of them is SSVNC.
