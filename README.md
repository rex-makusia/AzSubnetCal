# AzSubnetCal
The Official Repository of Azure Subnet Calculator CLI Edition

Run – Mode: Hosts
```yaml
==============================
 Azure VNet Subnet Calculator
==============================

Enter VNet CIDR: 10.0.0.0/16
Choose calculation mode:
1) Calculate by required hosts
2) Calculate by prefix length
Select option: 1

Enter number of hosts needed: 50

--- Calculation Results ---
VNet Address Space: 10.0.0.0/16
Subnet Mask: /25
Total IPs in Subnet: 128
Usable IPs: 123 (Azure reserves 5)
Subnet Range: 10.0.0.0 - 10.0.0.127

Other available subnets in VNet:
/25 - 10.0.0.128 - 10.0.0.255
/25 - 10.0.1.0   - 10.0.1.127
...
```

Run – Mode: Prefix
```yaml
==============================
 Azure VNet Subnet Calculator
==============================

Enter VNet CIDR: 10.0.0.0/16
Choose calculation mode:
1) Calculate by required hosts
2) Calculate by prefix length
Select option: 2

Enter prefix length: 24

--- Calculation Results ---
VNet Address Space: 10.0.0.0/16
Subnet Mask: /24
Total IPs in Subnet: 256
Usable IPs: 251 (Azure reserves 5)
First Subnet Range: 10.0.0.0 - 10.0.0.255

Other available subnets in VNet:
/24 - 10.0.1.0 - 10.0.1.255
/24 - 10.0.2.0 - 10.0.2.255
...
```