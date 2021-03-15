# Configuration Options

### Notes: 
* If you don't enable Ingress/Reverse Proxy on Collabora (It's not recommended as it is unsecure), in order for it to work you have to 
    * Remove `-o:ssl.termination=true -o:ssl.enable=false` from Extra Parameters.
    * Set Server Name to `hostIP:port` (The port you set for `NodePort`)
    * Set service type to `NodePort`
    * Set Port type to `HTTPS`
    * Disable certificate validation in the app you are going to use it.