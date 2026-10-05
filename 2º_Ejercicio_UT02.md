# 2º Ejercicio Práctico — UT 02
## Instalación Dual y Gestión del Arranque

**Módulo:** Implantación de Sistemas Operativos (1.º ASIR)

> **🎯 OBJETIVO:** Preparar un único disco virtual para que Windows 10 y Ubuntu convivan, realizar el particionado de forma consciente y verificar el arranque mediante GRUB.

---

### 1. Prepara Windows 10 para una instalación dual con Ubuntu
* **a.** Parte de una MV con Windows 10 Pro funcionando y muestra el estado inicial del Disco 0 desde Administración de discos.
* **b.** Reduce la partición `C:` y deja espacio **SIN ASIGNAR** para Ubuntu. Debe verse el valor introducido y el resultado final.
* **c.** Explica por qué el espacio destinado a Ubuntu debe quedar sin asignar y por qué no se utiliza un segundo disco virtual para esta práctica.

---

### 2. Instala Ubuntu en el mismo disco mediante particionado manual/personalizado
* **a.** Monta la ISO de Ubuntu y arranca la máquina virtual manteniendo el mismo modo de firmware utilizado por Windows.
* **b.** Selecciona la opción de particionado manual/personalizado (“Más opciones” o equivalente) y crea la partición Linux en el espacio libre.
* **c.** Completa la instalación de Ubuntu sin eliminar ni sobrescribir la instalación de Windows.
* **d.** Reinicia y demuestra que el menú GRUB permite arrancar tanto Ubuntu como Windows 10.

---

### 3. Verificación y documentación del arranque dual
* **a.** Arranca Ubuntu y muestra el sistema de archivos o las particiones para justificar dónde se ha instalado.
* **b.** Arranca Windows 10 desde GRUB y demuestra que sigue siendo funcional.
* **c.** Realiza un esquema sencillo del disco final indicando las particiones de Windows, la partición Linux y, si procede, la partición EFI.

---

> **📌 NOTA IMPORTANTE Y PAUTAS DE ENTREGA**
> - Entrega capturas de los pasos principales, no de cada clic. Debe apreciarse el **ANTES**, **DURANTE** y **DESPUÉS** de cada apartado.
> - Acompaña las capturas con una explicación breve y técnica de lo que has hecho y de qué resultado esperabas obtener.
> - En la mayoría de las capturas debe verse la barra de la máquina virtual, el nombre de la VM o algún elemento que permita identificar que el trabajo es tuyo.
> - Marca con flechas o recuadros las opciones importantes cuando sea necesario.
> - Redacción clara, vocabulario técnico correcto y revisión ortográfica antes de entregar.
> - **Entrega final en PDF con el nombre:** `Prueba_practica_UT02_Nombre_Apellido1_Apellido2.pdf`
