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

## 📦 Instalación y configuración

1. 🛠️ **Instala el paquete según tu distribución**

      Para sistemas basados en Debian/Ubuntu
      ```bash
      sudo dpkg -i wps-office*.deb
      ```

      Para sistemas basados en Red Hat/Fedora
      ```bash
      sudo dnf install wps-office*.rpm
      ```

2. 📂 **Copia las carpetas es_ES y es_MX**

      Ejecuta el siguiente comando desde la raíz (donde está la carpeta mui/)

      ```bash
      sudo cp -r mui/* /opt/kingsoft/wps-office/office6/mui/
      ```
      
3. ⚙️ **Cambia el idioma en la configuración y el modo multi ventana**
      
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
      wpsoffice\Application%20Settings\AppComponentMode=prome_independ
      wpsoffice\Application%20Settings\AppComponentModeInstall=prome_independ
      ```
4. 🏗️ **Copia los diccionarios de español**

   Ejecuta el siguiente comando desde la raíz (donde está la carpeta spellcheck/):
   ```bash
   sudo cp -r spellcheck/* /opt/kingsoft/wps-office/office6/dicts/spellcheck/
   ```
___
## 🚀 Resultado final

Una vez terminado el procesola interfaz estará en español 🇪🇸 ✨

![imagen](https://github.com/user-attachments/assets/686b8367-afbb-4487-a999-e61eef9d74c7)

![imagen](https://github.com/user-attachments/assets/6898a1e5-2caf-48a8-9136-a05217f24906)

![imagen](https://github.com/user-attachments/assets/d5ea0f02-e6d9-4b36-a739-fabd37626cd3)

___
## 🧠 Corrección ortográfica en español

Después de instalar WPS Office, puedes habilitar la corrección ortográfica para varios dialectos del español usando los diccionarios que ya están incluidos en este repositorio.

5. 🧩 **Activa la corrección ortográfica en español**

   ![imagen](https://github.com/user-attachments/assets/a297b315-32e8-42ba-a1cf-3d1383ac9a13)

   ![imagen](https://github.com/user-attachments/assets/ea83a4c3-27b0-4667-ac46-f00c28c77b0e)
   
---

🙌 

   Este tutorial fue creado para instalar WPS Office en español. Si te resultó útil, no dudes en dejar una estrella ⭐ en el repositorio o compartirlo con otros usuarios.
