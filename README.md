# Redes1_Practica1_202101728

# Manual Técnico - Práctica 1: Red Institucional de 3 Niveles

**Estudiante:** Iris Carolina Paz Guzman

**Carnet:** 202101728
**Curso:** Redes de Computadoras 1

## 1. Descripción de la Solución
Se diseñó e implementó una topología de red para un edificio de tres niveles, utilizando un esquema de conmutación jerárquico. La red permite la comunicación fluida entre departamentos de distintos pisos y el acceso a servidores centrales.

## 2. Estándares de Conectividad
* **Cableado Directo (TIA/EIA-568B):** Utilizado para conectar estaciones finales (PCs, Laptops) y servidores locales a sus respectivos switches de acceso.
* **Cableado Cruzado (Crossover):** Utilizado para el backbone de la red, interconectando switches de distribución y acceso entre niveles.

## 3. Direccionamiento IP (Red 192.178.28.0/24)
Basado en el carnet **202101728**, se utilizó el tercer octeto con valor **28**.

| Departamento | Rango de IPs | Máscara |
| :--- | :--- | :--- |
| Recepción (Piso 1) | 192.178.28.10 - .21 | 255.255.255.0 |
| Contabilidad (Piso 1) | 192.178.28.30 - .37 | 255.255.255.0 |
| Arqui / Urba (Piso 2) | 192.178.28.60 - .75 | 255.255.255.0 |
| Dirección / Civil (Piso 3) | 192.178.28.90 - .105 | 255.255.255.0 |
| Servidores Principales | 192.178.28.200 - .202 | 255.255.255.0 |

## 4. Configuración de Seguridad
Cada dispositivo de red (Switch) cuenta con:
* **Hostname** descriptivo según su área.
* **Contraseña de Enable:** 202101728.
* **Contraseña de VTY:** 202101728.

## 5. Resultados de Pruebas
Se validó la conectividad total mediante pruebas ICMP (Ping) exitosas entre el Nivel 1 y los servidores del Nivel 3.
