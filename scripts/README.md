@echo off
echo Iniciando proceso de mantenimiento y actualización...

:: Comprobación de la imagen de Windows (DISM)
:: echo Verificando la imagen de Windows...
:: DISM /Online /Cleanup-Image /ScanHealth
:: DISM /Online /Cleanup-Image /RestoreHealth

:: Escaneo y reparación de archivos del sistema
echo Escaneando y reparando archivos del sistema...
sfc /scannow

:: Actualización de programas usando winget
echo Actualizando programas...
winget upgrade --all --include-unknown

:: Limpieza de disco
echo Realizando limpieza de disco...
cleanmgr /sagerun:1

:: Limpieza de archivos temporales
echo Limpiando archivos temporales...
del /s /q %temp%\*
del /s /q C:\Windows\Temp\*
rd /s /q %systemdrive%\$Recycle.bin

echo Mantenimiento completado.
echo Eliminando el script...
del "%~f0"
