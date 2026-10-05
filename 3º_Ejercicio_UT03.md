# 3º Ejercicio Práctico — UT 03
## Configuración de Red en Windows y Linux

**Módulo:** Implantación de Sistemas Operativos (1.º ASIR)

> **🎯 OBJETIVO:** Configurar y comprobar los modos de red de VirtualBox (adaptador puente, Red NAT y red solo anfitrión), analizar la tabla ARP y las direcciones MAC, instalar roles y características en Windows Server y configurar la red de Ubuntu desde el terminal.

---

### 1. Red en Windows: adaptador puente, tabla ARP y dirección MAC
* **a.** Configura el adaptador de red de la MV de Windows en modo puente. Muestra la dirección IP de la MV y la tabla ARP tanto de la MV como de la máquina anfitrión.
* **b.** Haz ping desde la MV a la máquina anfitrión y vuelve a mostrar la tabla ARP de ambas máquinas.
* **c.** Desde la máquina anfitrión, localiza la IP y la dirección MAC de la MV. Confirma en VirtualBox (*Configuración > Red*) que esa MAC es la de la MV.
* **d.** Apaga la MV, modifica su dirección MAC y vuelve a arrancarla. Haz ping a la máquina anfitrión y comprueba que la MAC que aparece en su tabla ARP ha cambiado.

---

### 2. Red NAT en VirtualBox
* **a.** Crea una nueva Red NAT llamada **RED 100** con la red `192.168.100.0/24` y el DHCP habilitado.
* **b.** Conecta una MV de Windows a la RED 100 y comprueba que hay navegación por Internet tanto en la MV como en la máquina anfitrión.

---

### 3. Red solo anfitrión
* **a.** Crea una nueva red de anfitrión en VirtualBox con la IP `192.168.200.1`, máscara `255.255.255.0` y el DHCP habilitado.
* **b.** Cambia el adaptador de la MV a «Adaptador solo anfitrión», comprueba la IP que recibe la MV y haz ping en los dos sentidos entre la máquina anfitrión y la MV.

---

### 4. Roles y características en Windows Server
* **a.** En una MV de Windows Server, instala el rol de Servidor de fax y la característica Administración de directivas de grupo.

---

### 5. Red en Linux
* **a.** Conecta una MV de Ubuntu a una de las Redes NAT configuradas y modifica su IP desde el terminal para que pueda hacer ping a una MV de Windows de la misma red (la MV de Windows puede obtener su IP por DHCP).
* **b.** Muestra la tabla ARP de la máquina Ubuntu y señala la dirección MAC que corresponde a la MV de Windows del apartado anterior.

---

> **📌 NOTA IMPORTANTE Y PAUTAS DE ENTREGA**
> - Entrega capturas de los pasos principales, no de cada clic. Debe apreciarse el **ANTES**, **DURANTE** y **DESPUÉS** de cada apartado.
> - Acompaña las capturas con una explicación breve y técnica de lo que has hecho y de qué resultado esperabas obtener.
> - En la mayoría de las capturas debe verse la barra de la máquina virtual, el nombre de la VM o algún elemento que permita identificar que el trabajo es tuyo.
> - Marca con flechas o recuadros las opciones importantes cuando sea necesario.
> - Redacción clara, vocabulario técnico correcto y revisión ortográfica antes de entregar.
> - **Entrega final en PDF con el nombre:** `Prueba_practica_UT03_Nombre_Apellido1_Apellido2.pdf`
