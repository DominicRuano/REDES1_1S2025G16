# **Documentación Proyecto1 en Packet Tracer**

## **1. Tabla de Direcciones IP**

| **Vlan** | **Dispositivo** | **IP Asignada** | **Switch Conectado** |
|----------|-----------------|-----------------|----------------------|
|  1x      | PC0             | 192.168.100.10  | Switch Cliente01     |

## **2. Configuración de los Switches (script)**

### **Servidor**

Servidor VTP
Root bridge de STP

```bash
enable
configure terminal
spanning-tree vlan 1-4094 root primary
hostname servidor
vtp mode server
vtp version 2
vtp domain G16_technet
vtp password secure2025

vlan 11
 name Ventas
exit

vlan 21
 name Soporte
exit

vlan 31
 name Gerencia
exit

vlan 41
 name Seguridad
exit


interface range Fa0/1-3
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW1**

```bash
enable
configure terminal
hostname MSW1
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-6
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW2**

```bash
enable
configure terminal
hostname MSW2
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-6
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW3**

```bash
enable
configure terminal
hostname MSW3
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-6
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW4**

```bash
enable
configure terminal
hostname MSW4
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-6
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW5**

```bash
enable
configure terminal
hostname MSW5
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-4
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW6**

```bash
enable
configure terminal
hostname MSW6
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-5
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW7**

```bash
enable
configure terminal
hostname MSW7
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-4
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW9**

```bash
enable
configure terminal
hostname MSW9
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-6
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW10**

```bash
enable
configure terminal
hostname MSW10
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-6
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

interface range fa0/1-3
channel-group 1 mode Desirable
exit
 
interface port-channel 1
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **MSW11**

```bash
enable
configure terminal
hostname MSW11
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/4-5
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

interface range fa0/1-3
channel-group 1 mode Desirable
exit
 
interface port-channel 1
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

end

wr
```

### **SW0**

```bash
enable
configure terminal
hostname SW0
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-5
switchport mode trunk
exit

end

wr
```

### **SW1**

```bash
enable
configure terminal
hostname SW1
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-2
switchport mode trunk
exit

interface FastEthernet0/11
switchport mode access
switchport access vlan 11
exit

interface FastEthernet0/12
switchport mode access
switchport access vlan 31
exit

end

wr
```

### **SW2**

```bash
enable
configure terminal
hostname SW2
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface Fa0/1
switchport mode trunk
exit

interface FastEthernet0/11
switchport mode access
switchport access vlan 41
exit

end

wr
```

### **SW3**

```bash
enable
configure terminal
hostname SW3
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface Fa0/1
switchport mode trunk
exit

interface FastEthernet0/11
switchport mode access
switchport access vlan 21
exit

end

wr
```

### **SW4**

```bash
enable
configure terminal
hostname SW4
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface Fa0/1
switchport mode trunk
exit

interface FastEthernet0/11
switchport mode access
switchport access vlan 31
exit

interface FastEthernet0/12
switchport mode access
switchport access vlan 11
exit

end

wr
```

### **SW5**

```bash
enable
configure terminal
hostname SW5
vtp mode transparent
vtp version 2
vtp domain G16_technet
vtp password secure2025

vlan 51
 name recepcion
 exit

interface Fa0/1
 switchport mode trunk
 exit

interface FastEthernet0/11
 switchport mode access
 switchport access vlan 51
 exit

interface FastEthernet0/12
 switchport mode access
 switchport access vlan 51
 exit

interface FastEthernet0/13
 switchport mode access
 switchport access vlan 51
 exit

interface FastEthernet0/14
 switchport mode access
 switchport access vlan 51
 exit

end

wr
```

### **SW8**

```bash
enable
configure terminal
hostname SW8
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-2
 switchport mode trunk
 exit

interface FastEthernet0/11
 switchport mode access
 switchport access vlan 41
 exit

interface FastEthernet0/12
 switchport mode access
 switchport access vlan 11
 exit

end

wr
```

### **SW9**

```bash
enable
configure terminal
hostname SW9
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-2
 switchport mode trunk
 exit

interface FastEthernet0/11
 switchport mode access
 switchport access vlan 41
 exit

interface FastEthernet0/12
 switchport mode access
 switchport access vlan 21
 exit

end

wr
```

### **SW10**

```bash
enable
configure terminal
hostname SW10
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-2
 switchport mode trunk
 exit

interface FastEthernet0/11
 switchport mode access
 switchport access vlan 21
 exit

interface FastEthernet0/12
 switchport mode access
 switchport access vlan 11
 exit

interface FastEthernet0/13
 switchport mode access
 switchport access vlan 31
 exit

end

wr
```
