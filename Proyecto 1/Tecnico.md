# **Documentación Proyecto1 en Packet Tracer**

## **1. Tabla de Direcciones IP**

| **Vlan** | **Dispositivo** | **IP Asignada** | **Switch Conectado** |
|----------|-----------------|-----------------|----------------------|
|  11      | VENTAS 1        | 192.168.11.11   | SW4                  |
|----------|-----------------|-----------------|----------------------|
|  11      | VENTAS 2        | 192.168.11.12   | SW8                  |
|----------|-----------------|-----------------|----------------------|
|  11      | VENTAS 3        | 192.168.11.13   | SW10                 |
|----------|-----------------|-----------------|----------------------|
|  11      | VENTAS 4        | 192.168.11.14   | SW7                  |
|----------|-----------------|-----------------|----------------------|
|  11      | VENTAS 5        | 192.168.11.15   | SW1                  |
|----------|-----------------|-----------------|----------------------|
|  21      | SOPORTE 1       | 192.168.21.11   | SW3                  |
|----------|-----------------|-----------------|----------------------|
|  21      | SOPORTE 2       | 192.168.21.12   | SW9                  |
|----------|-----------------|-----------------|----------------------|
|  21      | SOPORTE 3       | 192.168.21.13   | SW10                 |
|----------|-----------------|-----------------|----------------------|
|  21      | SOPORTE 4       | 192.168.21.14   | SW6                  |
|----------|-----------------|-----------------|----------------------|
|  21      | SOPORTE 5       | 192.168.21.15   | SW11                 |
|----------|-----------------|-----------------|----------------------|
|  31      | GERENCIA 1      | 192.168.31.11   | SW4                  |
|----------|-----------------|-----------------|----------------------|
|  31      | GERENCIA 2      | 192.168.31.12   | SW1                  |
|----------|-----------------|-----------------|----------------------|
|  31      | GERENCIA 3      | 192.168.31.13   | SW13                 |
|----------|-----------------|-----------------|----------------------|
|  31      | GERENCIA 4      | 192.168.31.14   | SW12                 |
|----------|-----------------|-----------------|----------------------|
|  31      | GERENCIA 5      | 192.168.31.15   | SW10                 |
|----------|-----------------|-----------------|----------------------|
|  41      | SEGURIDAD 1     | 192.168.41.11   | SW2                  |
|----------|-----------------|-----------------|----------------------|
|  41      | SEGURIDAD 2     | 192.168.41.12   | SW8                  |
|----------|-----------------|-----------------|----------------------|
|  41      | SEGURIDAD 3     | 192.168.41.13   | SW11                 |
|----------|-----------------|-----------------|----------------------|
|  41      | SEGURIDAD 5     | 192.168.41.15   | SW6                  |
|----------|-----------------|-----------------|----------------------|
|  41      | SEGURIDAD 6     | 192.168.41.16   | SW7                  |
|----------|-----------------|-----------------|----------------------|
|  41      | SEGURIDAD 7     | 192.168.41.17   | SW9                  |
|----------|-----------------|-----------------|----------------------|
|  51      | RECEPCION 1     | 192.168.51.11   | SW5                  |
|----------|-----------------|-----------------|----------------------|
|  51      | RECEPCION 2     | 192.168.51.12   | SW5                  |
|----------|-----------------|-----------------|----------------------|
|  51      | RECEPCION 3     | 192.168.51.13   | SW5                  |
|----------|-----------------|-----------------|----------------------|
|  51      | RECEPCION 4     | 192.168.51.14   | SW5                  |


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

### **MSW8**
```bash
MSW8
enable
configure terminal
hostname MSW8
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
channel-group 2 mode active
exit
 
interface port-channel 2
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

interface range fa0/1-3
channel-group 2 mode active
exit
 
interface port-channel 2
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


### **SW6**
```bash
enable
configure terminal
hostname SW6
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

interface FastEthernet0/12
switchport mode access
switchport access vlan 41
exit

end

wr

```
### **SW7**
```bash
enable
configure terminal
hostname SW7
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface Fa0/1
switchport mode trunk
exit


interface FastEthernet0/12
switchport mode access
switchport access vlan 11
exit

interface FastEthernet0/11
switchport mode access
switchport access vlan 41
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
### **SW11**
```bash
enable
configure terminal
hostname SW11
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-2
switchport mode trunk
exit

interface range Fa0/5-6
switchport mode trunk
exit

interface FastEthernet0/4
switchport mode access
switchport access vlan 21
exit

interface FastEthernet0/3
switchport mode access
switchport access vlan 41
exit

end

wr

```

### **SW12**
```bash
enable
configure terminal
hostname SW12
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-3
switchport mode trunk
exit

interface FastEthernet0/11
switchport mode access
switchport access vlan 31
exit


end

wr

```

### **SW13**
```bash
enable
configure terminal
hostname SW13
vtp mode client
vtp version 2
vtp domain G16_technet
vtp password secure2025

interface range Fa0/1-3
switchport mode trunk
exit

interface FastEthernet0/11
switchport mode access
switchport access vlan 31
exit


end

wr

```

