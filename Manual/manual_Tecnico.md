# 🖧 Proyecto 1 - NetCore Academy

## 👩‍🎓 Datos del Estudiante

* Nombre: Iris Carolina Paz Guzman
* Carnet: 202101728
* Curso: Redes de Computadoras 1
* Sección: A

---

## 🌐 1. Topología General

![Topología General](Topologia.png)

---

## 🏢 2. Topología por Edificio

### 🟥 Edificio A

![A](topoA.png)

### 🟪 Edificio B

![B](TopoB.png)

### 🟦 Edificio C

![C](TopoC.png)

### 🟩 Edificio D

![D](TopoD.png)

---

## 📡 3. VLANs

| VLAN | Nombre      |
| ---- | ----------- |
| 18   | ADMIN       |
| 28   | DOCENTES    |
| 38   | BIBLIOTECA  |
| 48   | LABORATORIO |
| 58   | VISITANTES  |

---

## 🌍 4. Direccionamiento IP

### 🟥 Edificio A

* Admin2 → 192.168.18.10
* Docencia → 192.168.28.11 - 13
* Lab → 192.168.48.41 - 42

### 🟪 Edificio B

* Admin1 → 192.168.18.11
* Docente → 192.168.28.21
* Biblioteca → 192.168.38.31 - 43

### 🟦 Edificio C

* Admin3 → 192.168.18.12
* Docentes → 192.168.28.31 - 32
* Biblioteca → 192.168.38.51

---

## 🖥️ 5. Comandos Utilizados

```bash
vlan 18
vlan 28
vlan 38
vlan 48
vlan 58

interface gig0/1
switchport mode trunk

show spanning-tree
show etherchannel summary
show interfaces trunk
```

---

# 🌳 6. STP (Spanning Tree)

## 🟥 Edificio A (ROOT)

![STP A](stpa.png)
![STP A2](stpa2.png)

👉 SW-A1 es Root Bridge

---

## 🟪 Edificio B

![STP B](stpB1.png)

---

## 🟦 Edificio C

![STP C](stpC1.png)

---

## 🟩 Edificio D

![STP D](stpD2.png)

---

# 🔗 7. EtherChannel

## 🟥 Edificio A

![EC A](etherchanela2.png)

## 🟪 Edificio B

![EC B1](herchannelB1.png)
![EC B2](etherchannelB2.png)

## 🟦 Edificio C

![EC C](ethernetchanelC4.png)

## 🟦 Edificio D

![EC C](ethernetchanelD4.png)

---

Comando:

```bash
show etherchannel summary
```

---

# 🔀 8. Trunks

## 🟥 Edificio A

![A1](trunkA1.png)
![A2](TrunkA2.png)
![A3](TrunkA3.png)

## 🟪 Edificio B

![B1](trunkB1.png)
![B2](trunkB2.png)
![B3](trunkB3.png)
![B4](trunkB4.png)

## 🟦 Edificio C

![C2](trunkc2.png)
![C3](trunkc3.png)

## 🟦 Edificio D

![C2](trunkD2.png)
![C3](trunkD3.png)


---

Comando:

```bash
show interfaces trunk
```

---

#  9. Presupuesto

| Equipo        | Cantidad | Precio | Subtotal |
| ------------- | -------- | ------ | -------- |
| Switch 2960   | 10       | Q3500  | Q35000   |
| Switch-PT     | 4        | Q2000  | Q8000    |
| Módulos fibra | 8        | Q800   | Q6400    |
| Cable UTP     | 200m     | Q5     | Q1000    |
| Fibra óptica  | 50m      | Q15    | Q750     |
| Conectores    | 1 lote   | Q500   | Q500     |

### TOTAL: Q51,650

---

#  10. Conclusiones

* Se implementaron VLANs correctamente
* STP configurado con root en SW-A1
* EtherChannel mejora redundancia
* Trunks permiten comunicación entre VLANs

---
