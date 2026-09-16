---
title: Error en Excel al copiar y pegar
date: 2026-09-16T12:06:00.000-04:00
---
Debido a una actualización que sacó Microsoft (KB5002914) para corregir vulnerabilidades, terminó afectando a la función de pegar en las celdas de Microsoft Excel, por lo que a continuación te adjunto la solución si usas la última versión de Windows 11 que no te permite visualizar la lista de actualizaciones, este comando solo sirve para  versiones MSI de Office 2016, 2019, 2021 y LTSC:

Cierra todos las aplicaciones de Microsoft Office y ejecuta el comando en una ventada CMD con privilegios de administrador:

```
"C:\Program Files\Common Files\Microsoft Shared\OFFICE16\Oarpmany.exe" /removereleaseinpatch "{90160000-0012-0000-1000-0000000FF1CE}" "{27882596-A8ED-4382-9C71-6CD2DD19F732}" "1033" "0"
```

Posteriormente abre Excel y prueba nuevamente copiar y pegar, el error ya deberia haberse corregido.

`"C:\Program Files\Common Files\Microsoft Shared\OFFICE16\Oarpmany.exe" /removereleaseinpatch "{90160000-0012-0000-1000-0000000FF1CE}" "{27882596-A8ED-4382-9C71-6CD2DD19F732}" "1033" "0"`
