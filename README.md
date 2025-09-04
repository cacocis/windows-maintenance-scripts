# windows-maintenance-scripts
Colección de scripts en Batch/CMD para automatización de mantenimiento en Windows

# 🛠️ Scripts de Automatización para Soporte IT

Una colección de scripts útiles para automatizar tareas de mantenimiento y diagnóstico en sistemas Windows.

## 📦 Scripts Disponibles

### 🔄 `scripts/maintenance/update.bat`
Este script automatiza la actualización de software y paquetes en sistemas Windows.

**Uso:**
1. Ejecutar como Administrador.
2. Seguir las instrucciones en pantalla.

**Comandos principales:**
```batch
@echo off
echo Iniciando actualización de paquetes...
winget upgrade --all
echo ¡Actualización completada!
pause
```

### 🧹 `scripts/maintenance/cleanup.bat`
Realiza una limpieza de archivos temporales y libera espacio en disco.

## 🚀 ¿Cómo Usar?
1. Descarga el script que necesites.
2. Haz clic derecho > "Ejecutar como administrador".

## 📝 Licencia
Este proyecto está bajo la Licencia MIT. Siéntete libre de usarlo y modificarlo.
