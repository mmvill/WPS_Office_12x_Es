# 🇪🇸 WPS Office 12.1 en Español para Linux

Este repositorio contiene los archivos necesarios para traducir **WPS Office 12.1** al idioma **español** en sistemas **Linux**. Incluye las carpetas `es_ES` y `es_MX` listas para integrarse con WPS Office antes de su instalación.

*Para un versión de WPS Office completa y actualizada se recomienda descargar el instalador desde el sitio chino.*

---

## 📝 Requisitos previos

- El idioma de la distribución debe ser español España
- Instalador de **WPS Office** para tu distribución Linux (descárgalo desde el [sitio oficial chino (ver. 12.1)](https://www.wps.cn) ó deste el [sitio official global (ver. 11.xx)](https://www.wps.com)
- Permisos de superusuario (`sudo`)
- Este repositorio clonado o descargado localmente

---

## 📦 Integración del idioma español

1. 📁 **Crea el directorio de idioma**

   Asegúrate de que la ruta donde van los archivos de idioma exista:

   ```bash
   sudo mkdir -p /opt/kingsoft/wps-office/office6/mui/

2. 📂 **Copia las carpetas es_ES y es_MX**

   Ejecuta el siguiente comando desde la raíz (donde está la carpeta mui/)

   ```bash
   sudo cp -r mui/* /opt/kingsoft/wps-office/office6/mui/
   ```

## 💾 Instalación de WPS Office

3. 📥 Descarga el instalador oficial

    .deb para Debian, Ubuntu, Linux Mint, etc.
    
    .rpm para Fedora, openSUSE, RHEL, etc.

5. 🛠️ Instala el paquete según tu distribución

      ```bash
      # Para sistemas basados en Debian/Ubuntu
      sudo dpkg -i wps-office*.deb

      # Para sistemas basados en Red Hat/Fedora
      sudo dnf install wps-office*.rpm```
---
## 🚀 Resultado final

Una vez terminado el proceso, al iniciar WPS Office, la interfaz estará en español 🇪🇸✨

   ![imagen](https://github.com/user-attachments/assets/686b8367-afbb-4487-a999-e61eef9d74c7)

   ![imagen](https://github.com/user-attachments/assets/6898a1e5-2caf-48a8-9136-a05217f24906)

   ![imagen](https://github.com/user-attachments/assets/d5ea0f02-e6d9-4b36-a739-fabd37626cd3)


---

## 🧠 Corrección ortográfica en español (Diccionarios)

Después de instalar WPS Office, puedes habilitar la corrección ortográfica para varios dialectos del español usando los diccionarios que ya están incluidos en este repositorio.


### 📦 Contenido del directorio `spellcheck/`

Este repositorio incluye múltiples carpetas con diccionarios listos para usar, como:

- `es_ES` → Español de España
- `es_MX` → Español de México
- `es_AR` → Español de Argentina
- `es_CO` → Español de Colombia
- *(y más, según el contenido del repositorio)*

---

### 🧭 Pasos para instalar los diccionarios


1. 🏗️ **Copia todas las carpetas del repositorio**

   Ejecuta el siguiente comando desde la raíz (donde está la carpeta spellcheck/):
   ```bash
   sudo cp -r spellcheck/* /opt/kingsoft/wps-office/office6/dicts/spellcheck/
   ```

2. 🔁 **Reinicia WPS Office (si estaba abierto)**

   Para que el programa reconozca los nuevos diccionarios

3. 🧩 **Activa la corrección ortográfica en español**

   Dentro de WPS Writer:
   ![imagen](https://github.com/user-attachments/assets/a297b315-32e8-42ba-a1cf-3d1383ac9a13)

   ![imagen](https://github.com/user-attachments/assets/ea83a4c3-27b0-4667-ac46-f00c28c77b0e)
---

🙌 Créditos

   Este proyecto fue creado para simplificar el proceso de localización de WPS Office en entornos Linux. Si te resultó útil, no dudes en dejar una estrella ⭐ en el repositorio o compartirlo con otros usuarios.
