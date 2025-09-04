# windows-maintenance-scripts
Colección de scripts en Batch/CMD para automatización de mantenimiento en Windows.

<!-- Una descripción más detallada y motivadora -->
**¡Automatiza tareas repetitivas y recupera tiempo para focusearte en lo que realmente importa!** Estos scripts fueron creados y probados en entornos reales durante mis experiencias como técnico en soporte IT.

---

## 🚀 Scripts Disponibles

| Script | Descripción | Uso |
| :--- | :--- | :--- |
| **`update.bat`** | Automatiza la actualización de software y paquetes usando Winget. | Ejecutar como **Administrador**. |
| **`cleanup.bat`** | Realiza una limpieza profunda de archivos temporales y libera espacio en disco. | Ejecutar como **Administrador**. |
| **`diagnostic.bat`** | Ejecuta diagnósticos básicos del sistema (RAM, disco duro). | Ejecutar como usuario normal. |

---

## 📦 ¿Cómo Usar?

1.  **Descarga** el script que necesites.
2.  **Haz clic derecho** sobre el archivo `.bat`.
3.  Selecciona **"Ejecutar como administrador"** (para scripts de mantenimiento).
4.  **Sigue las instrucciones** en la ventana de comandos.

---

## 🛠️ Detalles Técnicos

### **`update.bat`**
Este script automatiza la actualización de software usando Winget, el gestor de paquetes de Microsoft.

**Comandos principales:**
```batch
@echo off
echo [INFO] Verificando actualizaciones disponibles...
winget upgrade --all --include-unknown
echo [INFO] ¡Proceso de actualización completado!
pause
```

### **`cleanup.bat`**
Limpia archivos temporales de sistema y de usuario utilizando la utilidad `cleanmgr` y comandos `del`.

---

## ❓ Preguntas Frecuentes

**¿Son seguros estos scripts?**
Sí, todos los scripts están escritos con comandos nativos de Windows y son de código abierto. Siempre se recomienda revisar el código antes de ejecutarlo.

**¿Necesito instalar algo?**
El script `update.bat` requiere tener **Winget** instalado (viene por defecto en Windows 11 y versiones modernas de Win10).

---

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Esto significa que puedes usarlo, modificarlo y distribuirlo libremente.

---

## 👨‍💻 Acerca del Autor

Soy un Técnico en Soporte IT apasionado por la automatización y la optimización de procesos. Puedes encontrar más sobre mi experiencia y proyectos en mi portfolio: **[https://cacocis.github.io](https://cacocis.github.io)**

*¿Encontraste útil este script? ¡Déjale una estrella ⭐ a este repositorio!*
