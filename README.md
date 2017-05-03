Using a Service Catalog and VMware Custom Specification, we can allow user to enter the IP for the VM in the service dialog.

The VM template is required to have open-vm-tools installed and enabled. 

How this works
===
* As part of the Service Catalog Item, we define the basic information in the Request Info -> Customize -> Specification, such as domain name and DNS information. 
* In the Service Dialog, the IP is provided using the `option_0_ip_addr` field name in the dialog.
* Upon boot up, the vmtoolsd will start and configure the VM with the static IP.

