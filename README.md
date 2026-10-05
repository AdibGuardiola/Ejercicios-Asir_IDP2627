# Ejercicios Prácticos - Implantación de Sistemas Operativos (1.º ASIR) 💻🐧🪟

Repositorio con los **enunciados de las pruebas prácticas** del módulo **Implantación de Sistemas Operativos (IDP 26/27)** para 1.º de ASIR (Administración de Sistemas Informáticos en Red).

---

## 📋 Índice de Ejercicios Prácticos

- [1º Ejercicio Práctico - UT 01: Virtualización e instalación de sistemas operativos](./1º_Ejercicio_UT01.md)
- [2º Ejercicio Práctico - UT 02: Instalación dual y gestión del arranque](./2º_Ejercicio_UT02.md)
- [3º Ejercicio Práctico - UT 03: Configuración de red en Windows y Linux](./3º_Ejercicio_UT03.md)
- [4º Ejercicio Práctico - UT 04: Instalación dual, arranque y particionado](./4º_Ejercicio_UT04.md)

---

## 1º Ejercicio Práctico — UT 01
### Virtualización e Instalación de Sistemas Operativos

> **🎯 OBJETIVO:** Demostrar que sabes crear y configurar máquinas virtuales, realizar instalaciones atendidas y completar la integración básica con VirtualBox.

#### 1. Crea una máquina virtual para instalar Ubuntu 24.04 de forma atendida
* **a.** Asigna 4096 MB de RAM y 2 procesadores. Deja desactivada la instalación desatendida y muestra la configuración antes de arrancar.
* **b.** Crea un disco virtual de 40 GB y selecciona de forma razonada EFI o BIOS antes de iniciar la instalación.
* **c.** Inicia el instalador, configura idioma, teclado, usuario y contraseña y completa la instalación hasta llegar al escritorio.
* **d.** Instala Guest Additions y comprueba al menos una función de integración, como redimensionado de pantalla o portapapeles bidireccional.

#### 2. Crea una máquina virtual para Windows Server 2022 e inicia una instalación atendida
* **a.** Configura 5000 MB de RAM, 2 procesadores y un disco de 50 GB.
* **b.** Selecciona correctamente la ISO, deja desactivada la instalación desatendida y explica la diferencia práctica entre arrancar con EFI o BIOS.
* **c.** Instala Windows Server 2022 con entorno gráfico hasta acceder al escritorio del servidor.
* **d.** Instala Guest Additions y verifica que la VM queda integrada correctamente con VirtualBox.

#### 3. Comprobación final de las máquinas virtuales
* **a.** Presenta una captura de la configuración final de Ubuntu y otra de Windows Server donde se vean RAM, CPU, disco y firmware.
* **b.** Explica en 5-8 líneas qué diferencias has observado entre una instalación atendida y una instalación automatizada/desatendida.
* **c.** Incluye una tabla resumen con nombre de VM, sistema operativo, RAM, CPU, disco, firmware y estado de Guest Additions.

> **📌 NOTA IMPORTANTE Y PAUTAS DE ENTREGA**
> - Entrega capturas de los pasos principales, no de cada clic. Debe apreciarse el **ANTES**, **DURANTE** y **DESPUÉS** de cada apartado.
> - Acompaña las capturas con una explicación breve y técnica de lo que has hecho y de qué resultado esperabas obtener.
> - En la mayoría de las capturas debe verse la barra de la máquina virtual, el nombre de la VM o algún elemento que permita identificar que el trabajo es tuyo.
> - Marca con flechas o recuadros las opciones importantes cuando sea necesario.
> - Redacción clara, vocabulario técnico correcto y revisión ortográfica antes de entregar.
> - **Entrega final en PDF con el nombre:** `Prueba_practica_UT01_Nombre_Apellido1_Apellido2.pdf`

---

## 2º Ejercicio Práctico — UT 02
### Instalación Dual y Gestión del Arranque

> **🎯 OBJETIVO:** Preparar un único disco virtual para que Windows 10 y Ubuntu convivan, realizar el particionado de forma consciente y verificar el arranque mediante GRUB.

#### 1. Prepara Windows 10 para una instalación dual con Ubuntu
* **a.** Parte de una MV con Windows 10 Pro funcionando y muestra el estado inicial del Disco 0 desde Administración de discos.
* **b.** Reduce la partición `C:` y deja espacio **SIN ASIGNAR** para Ubuntu. Debe verse el valor introducido y el resultado final.
* **c.** Explica por qué el espacio destinado a Ubuntu debe quedar sin asignar y por qué no se utiliza un segundo disco virtual para esta práctica.

#### 2. Instala Ubuntu en el mismo disco mediante particionado manual/personalizado
* **a.** Monta la ISO de Ubuntu y arranca la máquina virtual manteniendo el mismo modo de firmware utilizado por Windows.
* **b.** Selecciona la opción de particionado manual/personalizado (“Más opciones” o equivalente) y crea la partición Linux en el espacio libre.
* **c.** Completa la instalación de Ubuntu sin eliminar ni sobrescribir la instalación de Windows.
* **d.** Reinicia y demuestra que el menú GRUB permite arrancar tanto Ubuntu como Windows 10.

#### 3. Verificación y documentación del arranque dual
* **a.** Arranca Ubuntu y muestra el sistema de archivos o las particiones para justificar dónde se ha instalado.
* **b.** Arranca Windows 10 desde GRUB y demuestra que sigue siendo funcional.
* **c.** Realiza un esquema sencillo del disco final indicando las particiones de Windows, la partición Linux y, si procede, la partición EFI.

> **📌 NOTA IMPORTANTE Y PAUTAS DE ENTREGA**
> - Entrega capturas de los pasos principales, no de cada clic. Debe apreciarse el **ANTES**, **DURANTE** y **DESPUÉS** de cada apartado.
> - Acompaña las capturas con una explicación breve y técnica de lo que has hecho y de qué resultado esperabas obtener.
> - En la mayoría de las capturas debe verse la barra de la máquina virtual, el nombre de la VM o algún elemento que permita identificar que el trabajo es tuyo.
> - Marca con flechas o recuadros las opciones importantes cuando sea necesario.
> - Redacción clara, vocabulario técnico correcto y revisión ortográfica antes de entregar.
> - **Entrega final en PDF con el nombre:** `Prueba_practica_UT02_Nombre_Apellido1_Apellido2.pdf`

---

## 3º Ejercicio Práctico — UT 03
### Configuración de Red en Windows y Linux

> **🎯 OBJETIVO:** Configurar y comprobar los modos de red de VirtualBox (adaptador puente, Red NAT y red solo anfitrión), analizar la tabla ARP y las direcciones MAC, instalar roles y características en Windows Server y configurar la red de Ubuntu desde el terminal.

#### 1. Red en Windows: adaptador puente, tabla ARP y dirección MAC
* **a.** Configura el adaptador de red de la MV de Windows en modo puente. Muestra la dirección IP de la MV y la tabla ARP tanto de la MV como de la máquina anfitrión.
* **b.** Haz ping desde la MV a la máquina anfitrión y vuelve a mostrar la tabla ARP de ambas máquinas.
* **c.** Desde la máquina anfitrión, localiza la IP y la dirección MAC de la MV. Confirma en VirtualBox (*Configuración > Red*) que esa MAC es la de la MV.
* **d.** Apaga la MV, modifica su dirección MAC y vuelve a arrancarla. Haz ping a la máquina anfitrión y comprueba que la MAC que aparece en su tabla ARP ha cambiado.

#### 2. Red NAT en VirtualBox
* **a.** Crea una nueva Red NAT llamada **RED 100** con la red `192.168.100.0/24` y el DHCP habilitado.
* **b.** Conecta una MV de Windows a la RED 100 y comprueba que hay navegación por Internet tanto en la MV como en la máquina anfitrión.

#### 3. Red solo anfitrión
* **a.** Crea una nueva red de anfitrión en VirtualBox con la IP `192.168.200.1`, máscara `255.255.255.0` y el DHCP habilitado.
* **b.** Cambia el adaptador de la MV a «Adaptador solo anfitrión», comprueba la IP que recibe la MV y haz ping en los dos sentidos entre la máquina anfitrión y la MV.

#### 4. Roles y características en Windows Server
* **a.** En una MV de Windows Server, instala el rol de Servidor de fax y la característica Administración de directivas de grupo.

#### 5. Red en Linux
* **a.** Conecta una MV de Ubuntu a una de las Redes NAT configuradas y modifica su IP desde el terminal para que pueda hacer ping a una MV de Windows de la misma red (la MV de Windows puede obtener su IP por DHCP).
* **b.** Muestra la tabla ARP de la máquina Ubuntu y señala la dirección MAC que corresponde a la MV de Windows del apartado anterior.

> **📌 NOTA IMPORTANTE Y PAUTAS DE ENTREGA**
> - Entrega capturas de los pasos principales, no de cada clic. Debe apreciarse el **ANTES**, **DURANTE** y **DESPUÉS** de cada apartado.
> - Acompaña las capturas con una explicación breve y técnica de lo que has hecho y de qué resultado esperabas obtener.
> - En la mayoría de las capturas debe verse la barra de la máquina virtual, el nombre de la VM o algún elemento que permita identificar que el trabajo es tuyo.
> - Marca con flechas o recuadros las opciones importantes cuando sea necesario.
> - Redacción clara, vocabulario técnico correcto y revisión ortográfica antes de entregar.
> - **Entrega final en PDF con el nombre:** `Prueba_practica_UT03_Nombre_Apellido1_Apellido2.pdf`

---

## 4º Ejercicio Práctico — UT 04
### Instalación Dual, Arranque y Particionado

> **🎯 OBJETIVO:** Realizar una instalación dual de Windows 10 y Ubuntu redimensionando la partición de Windows, recuperar el arranque UEFI desde Windows RE tras borrar la partición EFI y particionar un segundo disco MBR con particiones primarias, extendida y lógicas.

#### 1. Instalación dual de Windows 10 y Ubuntu
* **a.** Usando una MV de Windows 10 (UEFI o MBR, como prefieras), realiza los pasos necesarios para hacer una instalación dual con Ubuntu.
* **b.** Debe verse el proceso de redimensión de la partición de Windows (no vale usar una MV con la partición ya redimensionada).
* **c.** Es obligatorio elegir el método de instalación personalizado de «Más opciones».

#### 2. Recuperación del arranque en UEFI
* **a.** Usando una MV de Windows 10 (UEFI), borra la partición EFI con el método que prefieras.
* **b.** Realiza los cambios necesarios para recuperar el arranque del sistema desde Windows RE.

#### 3. Particionado de un segundo disco MBR
* **a.** En la misma MV de Windows 10 (UEFI), añade un segundo disco de tipo MBR de 60 GB.
* **b.** Crea en este orden: dos particiones primarias de 10 GB, una partición extendida de 30 GB con dos unidades lógicas de 15 GB y una partición primaria con el espacio restante. Puedes usar el método y el software que prefieras.

> **📌 NOTA IMPORTANTE Y PAUTAS DE ENTREGA**
> - Entrega capturas de los pasos principales, no de cada clic. Debe apreciarse el **ANTES**, **DURANTE** y **DESPUÉS** de cada apartado.
> - Acompaña las capturas con una explicación breve y técnica de lo que has hecho y de qué resultado esperabas obtener.
> - En la mayoría de las capturas debe verse la barra de la máquina virtual, el nombre de la VM o algún elemento que permita identificar que el trabajo es tuyo.
> - Marca con flechas o recuadros las opciones importantes cuando sea necesario.
> - Redacción clara, vocabulario técnico correcto y revisión ortográfica antes de entregar.
> - **Entrega final en PDF con el nombre:** `Prueba_practica_UT04_Nombre_Apellido1_Apellido2.pdf`
