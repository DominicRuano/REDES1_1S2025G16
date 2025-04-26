# **Documentación Proyecto2 en Packet Tracer**

## **1. Calculo de subnetting**

### **VLSM CUNDECH**

| **Subred**  | **No.hosts** | **IP de red**      | **Mascara**     | **Primer**     | **Ultimo**     | **Broadcast**  |
|-------------|--------------|--------------------|-----------------|----------------|----------------|----------------|
| Biblioteca  | 126          | 192.168.16.0 /25   | 255.255.255.128 | 192.168.16.1   | 192.168.16.126 | 192.168.16.127 |
| Estudiantes | 62           | 192.168.16.128 /26 | 255.255.255.192 | 192.168.16.129 | 192.168.16.190 | 192.168.16.191 |
| Docentes    | 30           | 192.168.16.192 /27 | 255.255.255.224 | 192.168.16.193 | 192.168.16.222 | 192.168.16.223 |
| Seguridad   | 6            | 192.168.16.224 /29 | 255.255.255.248 | 192.168.16.225 | 192.168.16.230 | 192.168.16.231 |

### **VLSM CUNOROC**

| **Subred**  | **No.hosts** | **IP de red**      | **Mascara**     | **Primer**     | **Ultimo**     | **Broadcast**  |
|-------------|--------------|--------------------|-----------------|----------------|----------------|----------------|
| Biblioteca  | 126          | 192.168.16.0 /25   | 255.255.255.128 | 192.168.16.1   | 192.168.16.126 | 192.168.16.127 |
| Estudiantes | 62           | 192.168.16.128 /26 | 255.255.255.192 | 192.168.16.129 | 192.168.16.190 | 192.168.16.191 |
| Docentes    | 30           | 192.168.16.192 /27 | 255.255.255.224 | 192.168.16.193 | 192.168.16.222 | 192.168.16.223 |
| Seguridad   | 14           | 192.168.16.224 /28 | 255.255.255.240 | 192.168.16.225 | 192.168.16.238 | 192.168.16.239 |

### **VLSM CUNOC**

| **Subred**  | **No.hosts** | **IP de red**      | **Mascara**     | **Primer**     | **Ultimo**     | **Broadcast**  |
|-------------|--------------|--------------------|-----------------|----------------|----------------|----------------|
| Biblioteca  | 62           | 172.16.16.0 /26    | 255.255.255.192 | 172.16.16.1    | 172.16.16.62   | 172.16.16.63   |
| Estudiantes | 62           | 172.16.16.64 /26   | 255.255.255.192 | 172.16.16.65   | 172.16.16.126  | 172.16.16.127  |
| Docentes    | 62           | 172.16.16.128 /26  | 255.255.255.192 | 172.16.16.129  | 172.16.16.190  | 172.16.16.191  |
| Seguridad   | 6            | 172.16.16.192 /29  | 255.255.255.248 | 172.16.16.193  | 172.16.16.198  | 172.16.16.199  |

### **VLSM CUM**

| **Subred**  | **No.hosts** | **IP de red**      | **Mascara**     | **Primer**     | **Ultimo**     | **Broadcast**  |
|-------------|--------------|--------------------|-----------------|----------------|----------------|----------------|
| Biblioteca  | 126          | 192.158.16.0 /25   | 255.255.255.128 | 192.158.16.1   | 192.158.16.126 | 192.158.16.127 |
| Estudiantes | 62           | 192.158.16.128 /26 | 255.255.255.192 | 192.158.16.129 | 192.158.16.190 | 192.158.16.191 |
| Docentes    | 30           | 192.158.16.192 /27 | 255.255.255.224 | 192.158.16.193 | 192.158.16.222 | 192.158.16.223 |
| Seguridad   | 14           | 192.158.16.224 /28 | 255.255.255.240 | 192.158.16.225 | 192.158.16.238 | 192.158.16.239 |

## **. Tabla de Direcciones IP** (sin terminar)

| **Vlan** | **Dispositivo** | **IP Asignada**    | **Default Gateway**  |
|----------|-----------------|--------------------|----------------------|
|  11      | Estudiante 7    | 192.168.16.136 /26 | 192.168.16.129       |
|  11      | Estudiante 6    | 192.168.16.135 /26 | 192.168.16.129       |
|  11      | Estudiante 5    | 192.158.16.130 /26 | 192.158.16.129       |
|  11      | Estudiante 4    | ??                 |                      |
|  11      | Estudiante 3    | 192.168.16.132 /26 | 192.168.16.129       |
|  11      | Estudiante 2    | 172.16.16.67 /26   | 172.16.16.65         |
|  11      | Estudiante 1    | 172.16.16.66 /26   | 172.16.16.65         |
|  21      | Docente 7       | 192.168.16.200 /27 | 192.168.16.193       |
|  21      | Docente 6       | 192.168.16.199 /27 | 192.168.16.193       |
|  21      | Docente 5       | 192.158.16.194 /27 | 192.158.16.193       |
|  21      | Docente 4       | ??                 |                      |
|  21      | Docente 3       | 192.168.16.196 /27 | 192.168.16.193       |
|  21      | Docente 2       | 172.16.16.131 /26  | 172.16.16.129        |
|  21      | Docente 1       | 172.16.16.130 /26  | 172.16.16.129        |
|  21      | Seguridad 4     | 172.16.16.194 /29  | 172.16.16.193        |
|  31      | Seguridad 3     | 192.168.16.228 /28 | 192.168.16.225       |
|  31      | Seguridad 2     | 192.168.16.227 /29 | 192.168.16.225       |
|  31      | Seguridad 1     | 192.158.16.226 /28 | 192.158.16.225       |
|  41      | Biblioteca 4    | 192.168.16.5 /25   | 192.168.16.1         |
|  41      | Biblioteca 3    | 192.168.16.4 /25   | 192.168.16.1         |
|  41      | Biblioteca 2    | 192.158.16.2 /25   | 192.158.16.1         |
|  41      | Biblioteca 1    | 192.168.16.2 /25   | 192.168.16.1         |
|  41      | Servidor 0      | 192.120.16.11/25   | 192.120.16.1         |
|  41      | Servidor 1      | 192.121.16.11/25   | 192.121.16.1         |
|  41      | Servidor 2      | 192.122.16.11/25   | 192.122.16.1         |

## **. Capturas de la implementación de las topologías**

### Topologia completa

![Imagen Topologia completa](./images/Complete.png)

### CUNDECH

![Imagen area CUNDECH](./images/CUNDECH.png)

### CUNOROC

![Imagen area CUNOROC](./images/CUNOROC.png)

### CUNOC

![Imagen area CUNOC](./images/CUNOC.png)

### CENTRAL

![Imagen area CENTRAL](./images/CENTRAL.png)

### CUM

![Imagen area CUM](./images/CUM.png)

## **. Configuración de los Switches (script)** (sin terminar)

### **R0**

```bash
ena
config t
hostname R0

router rip
version 2
no auto-summary
network 172.16.21.0
network 172.16.22.0
network 172.16.16.0
network 192.168.16.0

interface GigabitEthernet0/0.11
encapsulation dot1Q 11
ip address 192.168.16.129 255.255.255.192
no shutdown

interface GigabitEthernet0/0.21
encapsulation dot1Q 21
ip address 192.168.16.193 255.255.255.224
no shutdown

interface GigabitEthernet0/0.31
encapsulation dot1Q 31
ip address 192.168.16.225 255.255.255.240
no shutdown

interface GigabitEthernet0/0.41
encapsulation dot1Q 41
ip address 192.168.16.1 255.255.255.128
no shutdown

interface GigabitEthernet0/0
no shutdown

interface Serial0/1/0
ip address 172.16.21.2 255.255.255.252
no shutdown

interface Serial0/1/1
ip address 172.16.22.2 255.255.255.252
no shutdown
end

wr

```

### **R1**

```bash
ena
config t
hostname R1

router rip
version 2
no auto-summary
network 10.0.3.0
network 172.16.21.0
network 11.0.0.0

interface gig0/0
ip address 10.0.3.2 255.255.255.252
no shutdown

interface Serial0/1/1
ip address 172.16.21.1 255.255.255.252
clock rate 64000
no shutdown

interface serial0/1/0
ip address 172.16.31.1 255.255.255.252
no shutdown
end

wr
```

### **R2**

```bash
ena
config t
hostname R2

interface serial0/1/0
ip address 172.16.31.2 255.255.255.252
no shutdown

interface serial0/1/1
ip address 172.16.22.1 255.255.255.252
no shutdown
exit

router rip
version 2
no auto-summary
network 172.16.31.0
network 172.16.22.0
exit

router ospf 1
redistribute rip subnets
redistribute ospf 1
redistribute ospf 1 metric 2


end
wr
```

### **R3**

```bash
interface GigabitEthernet0/0
ip address 10.16.11.254 255.0.0.0

exit
interface GigabitEthernet0/0
no shutdown


interface GigabitEthernet0/1
no ip address
ip address 11.10.16.253 255.0.0.0
no shutdown

router ospf 1
network 10.16.11.0 0.255.255.255 area 0
network 11.10.16.0 0.255.255.255 area 0

configure terminal
ip routing

router ospf 1
router-id 4.4.4.4
network 11.0.0.0 0.255.255.255 area 0
exit

```

### **R4**

```bash
ena
config t
hostname R4

interface GigabitEthernet0/1.41
encapsulation dot1q 41
ip address 192.158.16.126 255.255.255.128
standby 41 ip 192.158.16.1
standby 41 priority 110
standby 41 preempt
no shutdown
exit

interface GigabitEthernet0/1.11
encapsulation dot1q 11
ip address 192.158.16.190 255.255.255.192
standby 11 ip 192.158.16.129
standby 11 priority 110
standby 11 preempt
no shutdown
exit

interface GigabitEthernet0/1.21
encapsulation dot1q 21
ip address 192.158.16.222 255.255.255.224
standby 21 ip 192.158.16.193
standby 21 priority 110
standby 21 preempt
no shutdown
exit

interface GigabitEthernet0/1.31
encapsulation dot1q 31
ip address 192.158.16.238 255.255.255.240
standby 31 ip 192.158.16.225
standby 31 priority 110
standby 31 preempt
no shutdown
exit

interface GigabitEthernet0/1
no shutdown
exit

exit
write memory
```

### **R4.old**

```bash
ena
config t
hostname R4

int g0/0
ip add 192.158.16.2 255.255.255.0
no sh

standby version 2
standby 2 ip 192.158.16.1
standby 2 priority 150
standby 2 preempt
exit


interface GigabitEthernet0/1.41
encapsulation dot1q 41
ip address 192.158.16.4 255.255.255.128
no shutdown
exit

interface GigabitEthernet0/1.11
encapsulation dot1q 11
ip address 192.158.16.129 255.255.255.192
no shutdown
exit

interface GigabitEthernet0/1.21
encapsulation dot1q 21
ip address 192.158.16.193 255.255.255.224
no shutdown
exit

interface GigabitEthernet0/1.31
encapsulation dot1q 31
ip address 192.158.16.225 255.255.255.240
no shutdown
exit

interface GigabitEthernet0/1
no shutdown
exit

exit
write memory
```

### **R5**

```bash
ena
config t
hostname R5

interface GigabitEthernet0/1.41
encapsulation dot1q 41
ip address 192.158.16.125 255.255.255.128
standby 41 ip 192.158.16.1
standby 41 priority 100
standby 41 preempt
no shutdown
exit

interface GigabitEthernet0/1.11
encapsulation dot1q 11
ip address 192.158.16.189 255.255.255.192
standby 11 ip 192.158.16.129
standby 11 priority 100
standby 11 preempt
no shutdown
exit

interface GigabitEthernet0/1.21
encapsulation dot1q 21
ip address 192.158.16.221 255.255.255.224
standby 21 ip 192.158.16.193
standby 21 priority 100
standby 21 preempt
no shutdown
exit

interface GigabitEthernet0/1.31
encapsulation dot1q 31
ip address 192.158.16.237 255.255.255.240
standby 31 ip 192.158.16.225
standby 31 priority 100
standby 31 preempt
no shutdown
exit

interface GigabitEthernet0/1
no shutdown
exit

exit
write memory
```

### **R5.old**

```bash
ena
config t
hostname R5

int g0/0
ip add 192.158.16.3 255.255.255.0
no sh

standby version 2
standby 2 ip 192.158.16.1

interface GigabitEthernet0/0.41
encapsulation dot1q 41
ip address 192.158.16.4 255.255.255.128
no shutdown
exit

interface GigabitEthernet0/0.11
encapsulation dot1q 11
ip address 192.158.16.129 255.255.255.192
no shutdown
exit

interface GigabitEthernet0/0.21
encapsulation dot1q 21
ip address 192.158.16.193 255.255.255.224
no shutdown
exit

interface GigabitEthernet0/0.31
encapsulation dot1q 31
ip address 192.158.16.225 255.255.255.240
no shutdown
exit

interface GigabitEthernet0/1
no shutdown
exit

exit
write memory

```

### **R7**

```bash
ena
config t
hostname R7

interface GigabitEthernet0/1.51
encapsulation dot1q 51
ip address 192.120.16.1 255.255.255.0
no shutdown
exit

interface GigabitEthernet0/1.61
encapsulation dot1q 61
ip address 192.121.16.1 255.255.255.0
no shutdown
exit

interface GigabitEthernet0/1.71
encapsulation dot1q 71
ip address 192.122.16.1 255.255.255.0
no shutdown
exit

interface GigabitEthernet0/1
no shutdown
exit

interface GigabitEthernet0/0
no shutdown
exit



end
write memory
```

### **MS0**

```bash
ena
config t
hostname MS0

vtp domain Grupo16
vtp password usac2025
vtp mode server

vlan 11
name Estudiantes

vlan 21
name Docentes

vlan 31
name Seguridad

vlan 41
name Biblioteca

interface range Fa0/1-5
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all
end

wr
```

### **MS1**

```bash
ena
config t
hostname MS1

vtp mode client
vtp version 2
vtp domain Grupo16
vtp password usac2025

ip routing

router rip
version 2
no auto-summary
network 172.16.16.0
network 10.0.1.0

interface vlan 11
ip address 172.16.16.126 255.255.255.192
standby 11 ip 172.16.16.65
standby 11 priority 110
standby 11 preempt
no shutdown

interface vlan 21
ip address 172.16.16.190 255.255.255.192
standby 21 ip 172.16.16.129
standby 21 priority 110
standby 21 preempt
no shutdown

interface vlan 31
ip address 172.16.16.198 255.255.255.248
standby 31 ip 172.16.16.193
standby 31 priority 110
standby 31 preempt
no shutdown

interface vlan 41
ip address 172.16.16.62 255.255.255.192
standby 41 ip 172.16.16.1
standby 41 priority 110
standby 41 preempt
no shutdown

interface Fa0/1
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all

interface Fa0/2
no switchport
ip address 10.0.1.1 255.255.255.252
no shutdown
end

wr
```

### **MS2**

```bash
ena
config t
hostname MS2

vtp mode client
vtp version 2
vtp domain Grupo16
vtp password usac2025

ip routing

router rip
version 2
no auto-summary
network 172.16.16.0
network 10.0.2.0

interface vlan 11
ip address 172.16.16.125 255.255.255.192
standby 11 ip 172.16.16.65
standby 11 priority 100
standby 11 preempt
no shutdown

interface vlan 21
ip address 172.16.16.189 255.255.255.192
standby 21 ip 172.16.16.129
standby 21 priority 100
standby 21 preempt
no shutdown

interface vlan 31
ip address 172.16.16.197 255.255.255.248
standby 31 ip 172.16.16.193
standby 31 priority 100
standby 31 preempt
no shutdown

interface vlan 41
ip address 172.16.16.61 255.255.255.192
standby 41 ip 172.16.16.1
standby 41 priority 100
standby 41 preempt
no shutdown

interface Fa0/1
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all

interface Fa0/2
no switchport
ip address 10.0.2.1 255.255.255.252
no shutdown
end

wr
```

### **MS3**

```bash
ena
config t
hostname MS3

ip routing

router rip
version 2
no auto-summary
network 10.0.1.0
network 10.0.2.0
network 10.0.3.0
network 11.0.0.0

interface fa0/1
no switchport
ip address 10.0.1.2 255.255.255.252
no shutdown

interface fa0/2
no switchport
ip address 10.0.2.2 255.255.255.252
no shutdown

interface fa0/3
no switchport
ip address 10.0.3.1 255.255.255.252
no shutdown
end

wr
```

### **MS4**

```bash
ena
config t
ip routing
router ospf 1
network 11.10.16.0 0.255.255.255 area 0
network 12.10.16.0 0.0.0.255 area 0
network 13.10.16.0 0.0.0.255 area 0

vlan 16
name VLAN16
exit

interface range fastEthernet 0/2 - 4
switchport mode access
switchport access vlan 16
no shutdown
exit

show vlan brief
show interfaces status
show running-config interface range fastEthernet 0/2 - 4

interface vlan 16
ip address 12.10.16.1 255.0.0.0
no shutdown
exit

router ospf 1
network 12.10.16.0 0.255.255.255 area 0
exit

vlan 17
name VLAN17
exit

interface range fastEthernet 0/5 - 7
switchport mode access
switchport access vlan 17
no shutdown
exit

show vlan brief
show interfaces status
show running-config interface range fastEthernet 0/5 - 7

interface vlan 17
ip address 13.10.16.1 255.0.0.0
no shutdown
exit

router ospf 1
network 13.10.16.0 0.255.255.255 area 0
exit

configure terminal
interface FastEthernet0/1
no switchport
ip address 11.10.16.254 255.0.0.0
no shutdown
exit

interface FastEthernet0/5
no switchport
ip address 172.16.1.1 255.255.255.252
no shutdown
exit


router ospf 1
network 11.0.0.0 0.255.255.255 area 0
network 172.16.1.0 0.0.0.3 area 0

end
wr
```

### **MS5**

```bash
configure terminal
no router ospf 1
configure terminal
interface FastEthernet0/2
no switchport
ip address 172.16.1.2 255.255.255.252
no shutdown
exit
router ospf 1
router-id 5.5.5.5
network 172.16.1.0 0.0.0.3 area 0

configure terminal
interface FastEthernet0/6
no switchport
ip address 172.16.2.2 255.255.255.252
no shutdown
exit

router ospf 1
network 172.16.2.0 0.0.0.3 area 0
exit


end
wr
```

### **MS8**

```bash
enable
config t
Hostname MS8

vtp mode client
vtp version 2
vtp domain Grupo16
vtp password usac2025

ip routing

interface vlan 11
ip address 192.168.16.129 255.255.255.192
no shutdown

interface vlan 21
ip address 192.168.16.193 255.255.255.224
no shutdown

interface vlan 31
ip address 192.168.16.225 255.255.255.248
no shutdown

interface vlan 41
ip address 192.168.16.1 255.255.255.128
no shutdown

interface range Fa0/2-4
switchport trunk encapsulation dot1q
switchport mode trunk
switchport trunk allowed vlan all 
exit

exit
wr
```

### **Switch0**

```bash
ena
config t
hostname SW0

vtp domain Grupo16
vtp password usac2025
vtp mode server
vtp version 2
exit

configure terminal
vlan 51
name VLAN51
exit
vlan 61
name VLAN61
exit
vlan 71
name VLAN71
exit

interface fastEthernet 0/1 
switchport mode trunk
switchport trunk allowed vlan all
no shutdown
exit

interface fastEthernet 0/2  
switchport mode access
switchport access vlan 71

interface fastEthernet 0/3  
switchport mode access
switchport access vlan 51

interface fastEthernet 0/4  
switchport mode access
switchport access vlan 61

end
write memory
```

### **SW0**

```bash
ena
config t
hostname SW0

vtp domain Grupo16
vtp password usac2025
vtp mode client

interface Fa0/1
switchport mode trunk
exit

interface range Fa0/11-12
switchport mode acces
switchport access vlan 21
end

wr
```

### **SW1**

```bash
ena
config t
hostname SW1

vtp domain Grupo16
vtp password usac2025
vtp mode client

interface Fa0/1
switchport mode trunk
exit

interface range Fa0/11-12
switchport mode acces
switchport access vlan 11
end

wr
```

### **SW2**

```bash
ena
config t
hostname SW2

vtp domain Grupo16
vtp password usac2025
vtp mode client

interface range Fa0/1-2
switchport mode trunk
exit

interface Fa0/11
switchport mode acces
switchport access vlan 21
exit

exit
wr
```

### **SW3**

```bash
ena
config t
hostname SW3

vtp domain Grupo16
vtp password usac2025
vtp mode server

vlan 11
name Estudiantes

vlan 21
name Docentes

vlan 31
name Seguridad

vlan 41
name Biblioteca

interface range Fa0/1-2
switchport mode trunk
exit

interface Fa0/11
switchport mode acces
switchport access vlan 11
exit

exit
wr
```

### **SW4**

```bash
ena
config t
hostname SW4

vtp domain Grupo16
vtp password usac2025
vtp mode client

interface Fa0/1
switchport mode trunk
exit

interface Fa0/11
switchport mode acces
switchport access vlan 31
exit

interface Fa0/12
switchport mode acces
switchport access vlan 41
exit

exit
wr
```

### **SW5**

```bash
ena
config t
hostname SW5

vtp domain Grupo16
vtp password usac2025
vtp mode server
exit

configure terminal
vlan 11
name Estudiantes
exit
vlan 21
name Docentes
exit
vlan 31
name Seguridad
exit
vlan 41
name Biblioteca
exit

interface fastEthernet 0/14  
switchport mode access
switchport access vlan 11

interface fastEthernet 0/13  
switchport mode access
switchport access vlan 21

interface fastEthernet 0/12  
switchport mode access
switchport access vlan 31

interface fastEthernet 0/11  
switchport mode access
switchport access vlan 41


interface range fastEthernet 0/1-1 
switchport mode trunk
switchport trunk

end
write memory
```

### **SW6**

```bash
ena
config t
hostname SW6

vtp mode client
vtp version 2
vtp domain Grupo16
vtp password usac2025

interface range Fa0/1-2
switchport mode trunk
exit

interface Fa0/11
switchport mode acces
switchport access vlan 31
exit
interface range Fa0/12-13
switchport mode acces
switchport access vlan 41
exit

exit
wr
```

### **SW7**

```bash
ena
config t
hostname SW7

vtp domain Grupo16
vtp password usac2025
vtp mode server

vlan 11
name Estudiantes

vlan 21
name Docentes

vlan 31
name Seguridad

vlan 41
name Biblioteca

interface range Fa0/1-3
switchport mode trunk
exit

interface range Fa0/11-12
switchport mode acces
switchport access vlan 11
exit

exit
wr
```

### **SW8**

```bash
ena
config t
hostname SW8

vtp domain Grupo16
vtp password usac2025
vtp mode client

interface range Fa0/2-3
switchport mode trunk
exit

interface range Fa0/11-12
switchport mode acces
switchport access vlan 21
exit

exit
wr
```

### **SW9**

```bash
ena
config t
hostname SW9

vtp domain Grupo16
vtp password usac2025
vtp mode client

interface Fa0/1
switchport mode trunk
exit

interface Fa0/11
switchport mode acces
switchport access vlan 31
end

wr
```

### **R2 modificacion**

```bash
interface GigabitEthernet0/0
ip address 10.16.11.253 255.0.0.0

exit
interface GigabitEthernet0/0
no shutdown

router ospf 1
network 172.16.31.0 0.0.0.255 area 0
network 172.16.22.0 0.0.0.255 area 0
network 10.16.11.0 0.255.255.255 area 0

```

### **MS6**

```bash
ena
config t
ip routing
router ospf 1
network 12.10.16.0 0.255.255.255 area 0

ip routing
vlan 11
name VLAN11
exit
vlan 21
name VLAN21
exit
vlan 31
name VLAN31
exit
vlan 41
name VLAN41
exit

interface vlan 11
ip address 192.158.16.129 255.255.255.192
no shutdown
exit

interface vlan 21
ip address 192.158.16.193 255.255.255.224
no shutdown
exit

interface vlan 31
ip address 192.158.16.225 255.255.255.240
no shutdown
exit

interface vlan 41
ip address 192.158.16.4 255.255.255.128
no shutdown
exit

configure terminal
vlan 16
name OSPF_Switch_VLAN
exit

interface vlan 16
ip address 12.10.16.1 255.0.0.0
no shutdown
exit


interface range fastEthernet 0/1 - 3
description Link to OSPF Switch
switchport mode access
switchport access vlan 16
no shutdown
exit


interfaces status
show vlan brief

router ospf 1
router-id 6.6.6.6
network 192.158.16.129 0.0.0.63 area 0
network 192.158.16.193 0.0.0.31 area 0
network 192.158.16.225 0.0.0.15 area 0
network 192.158.16.4 0.0.0.127 area 0
network 12.10.16.1 255.0.0.0 area 0
exit


configure terminal
interface vlan16
ip address 12.10.16.2 255.0.0.0
exit
exit
```
### **R9**

```bash
ena
config t
int gi0/0
ip add 14.10.16.1 255.0.0.0
no shut
exit

int gi0/1
ip add 15.10.16.1 255.255.255.0
exit
exit
write memory

```
### **R10**

```bash
ena
config t
int gi0/1
ip add 192.168.16.225 255.255.255.0
no shut
exit

int gi0/0
ip add 15.10.16.2 255.255.255.0
speed 1000
exit
exit
write memory

```
### ****

```bash
```
### ****

```bash
```