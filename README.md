# 🇪🇸 WPS Office 12.1 en Español para Linux

Este repositorio contiene los archivos necesarios para traducir **WPS Office 12.1** al idioma **español** en sistemas **Linux**. Incluye las carpetas `es_ES` y `es_MX` listas para integrarse con WPS Office antes de su instalación.

*Para un versión de WPS Office completa y actualizada se recomienda descargar el instalador desde el sitio chino.*

---

## 📝 Requisitos previos

- El idioma de la distribución debe ser español España
- Instalador de **WPS Office** para tu distribución Linux (descárgalo desde el [sitio oficial chino (ver. 12.x)](https://www.wps.cn) ó deste el [sitio official global (ver. 11.x)](https://www.wps.com)
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
3. 🏠 Copiar la carpeta Kingsoft al directorio local del usuario

      Esto permite que los archivos de idioma también estén disponibles en tu espacio de usuario:

      ```bash
      cp -r Kingsoft ~/.local/
      ```

## 💾 Instalación de WPS Office

4. 🛠️ Instala el paquete según tu distribución

      Para sistemas basados en Debian/Ubuntu
      ```bash
      sudo dpkg -i wps-office*.deb
      ```

      Para sistemas basados en Red Hat/Fedora
      ```bash
      sudo dnf install wps-office*.rpm
      ```

5. ⚙️ Cambia el idioma en la configuración
      
      Edita el archivo de configuración de usuario para activar los cambios:
      ```bash
      nano ~/.config/Kingsoft/Office.conf
      ```

      Busca y modifica las líneas en las secciones [General] y [6.0] para que queden con estos valores exactos:
      ```bash
      [General]
      languages=es_ES
      [6.0]
      common\DefaultLanguage=3082
      common\Local\UILanguage=3082
      ```

---
# Aviso:

- Las pantallas individuales si estaran en español (Presentation, Spreadsheets, Write y PDF), pero la pantalla incial siempre estara en ingles.
- Se recomienda cambiar la configuracion de comportamiento de la palicacion para que WPS gestione las aplicaciones individualmente:
      
![imagen](https://github.com/user-attachments/assets/21366d80-7925-4ecd-8552-475dde11bf1f)
![imagen](https://github.com/user-attachments/assets/d7f70a20-3b2d-4310-b605-8f38e8d0d75b)
![imagen](https://github.com/user-attachments/assets/5f0161b2-6342-4545-a04d-9f48cf0c7192)
![imagen](https://github.com/user-attachments/assets/5c05053b-5320-4324-b7e9-1fb204233ebb)
      
- Cierrar todas las ventanas de WPS y abrir cualquier aplicacion, al presionar "+" abre un nuevo documento.
      
![imagen](https://github.com/user-attachments/assets/c43619fb-f955-417d-bba3-42d7a78a84b0)

## 🚀 Resultado final

Una vez terminado el procesola interfaz estará en español 🇪🇸 ✨

![imagen](https://github.com/user-attachments/assets/686b8367-afbb-4487-a999-e61eef9d74c7)

![imagen](https://github.com/user-attachments/assets/6898a1e5-2caf-48a8-9136-a05217f24906)

![imagen](https://github.com/user-attachments/assets/d5ea0f02-e6d9-4b36-a739-fabd37626cd3)

___
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

🙌 

   Este tutorial fue creado para instalar WPS Office en español. Si te resultó útil, no dudes en dejar una estrella ⭐ en el repositorio o compartirlo con otros usuarios.
