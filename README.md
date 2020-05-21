# Meraki ClientVPN split Tunnel Powershell Script
Powershell script that Configures a windows client with Meraki ClientVPN configuration details and uses split tunneling.  There are a few variables that need to be populated before this script will work.  Below is a list of variables:

     $vpnname = This is the name that will be displayed in the Network settings bar.

     $vpnserver = Either the IP or hostname of the MX firewall that the VPN will connect to.  Note that using the dynamic DNS name Meraki      provides will make sure this VPN profile works in the event of a firewall failover.

     $vpnkey = This is the shared secret key configured in the Meraki dashboard under Client VPN.

     $DestinationX = A remote subnet that tells Windows to send traffic over the tunnel.  Note that you need to add additional Destination 1...n variables, one for each remote subnet.
