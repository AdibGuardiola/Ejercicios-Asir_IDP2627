# 4º Ejercicio Práctico — UT 04
## Instalación Dual, Arranque y Particionado

**Módulo:** Implantación de Sistemas Operativos (1.º ASIR)

> **🎯 OBJETIVO:** Realizar una instalación dual de Windows 10 y Ubuntu redimensionando la partición de Windows, recuperar el arranque UEFI desde Windows RE tras borrar la partición EFI y particionar un segundo disco MBR con particiones primarias, extendida y lógicas.

---

### 1. Instalación dual de Windows 10 y Ubuntu
* **a.** Usando una MV de Windows 10 (UEFI o MBR, como prefieras), realiza los pasos necesarios para hacer una instalación dual con Ubuntu.
* **b.** Debe verse el proceso de redimensión de la partición de Windows (no vale usar una MV con la partición ya redimensionada).
* **c.** Es obligatorio elegir el método de instalación personalizado de «Más opciones».

---

### 2. Recuperación del arranque en UEFI
* **a.** Usando una MV de Windows 10 (UEFI), borra la partición EFI con el método que prefieras.
* **b.** Realiza los cambios necesarios para recuperar el arranque del sistema desde Windows RE.

---

### 3. Particionado de un segundo disco MBR
* **a.** En la misma MV de Windows 10 (UEFI), añade un segundo disco de tipo MBR de 60 GB.
* **b.** Crea en este orden: dos particiones primarias de 10 GB, una partición extendida de 30 GB con dos unidades lógicas de 15 GB y una partición primaria con el espacio restante. Puedes usar el método y el software que prefieras.

---

> **📌 NOTA IMPORTANTE Y PAUTAS DE ENTREGA**
> - Entrega capturas de los pasos principales, no de cada clic. Debe apreciarse el **ANTES**, **DURANTE** y **DESPUÉS** de cada apartado.
> - Acompaña las capturas con una explicación breve y técnica de lo que has hecho y de qué resultado esperabas obtener.
> - En la mayoría de las capturas debe verse la barra de la máquina virtual, el nombre de la VM o algún elemento que permita identificar que el trabajo es tuyo.
> - Marca con flechas o recuadros las opciones importantes cuando sea necesario.
> - Redacción clara, vocabulario técnico correcto y revisión ortográfica antes de entregar.
> - **Entrega final en PDF con el nombre:** `Prueba_practica_UT04_Nombre_Apellido1_Apellido2.pdf`
