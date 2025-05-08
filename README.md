GHOSTLINK

Ghostlink es un script en PowerShell que simula una amenaza persistente avanzada (APT) con fines educativos y de concienciación en ciberseguridad. Está diseñado para ser utilizado en entornos controlados como parte de ejercicios Red Team, formación interna o simulaciones de ataques USB.

---

## 🧩 Características

- **Persistencia automática:** mediante claves de registro y tareas programadas.
- **Instalación oculta:** en rutas del sistema poco inspeccionadas.
- **Ejecución silenciosa:** sin mostrar consola ni ventanas al usuario.
- **Control remoto:** mediante conexión TCP (puerto configurable).
- **Desinstalación remota:** con comando `uninstall` o parámetro `-Action uninstall`.
- **Detección y limpieza profunda:** elimina rastros, tareas, archivos y conexiones.

---

## ⚙️ Archivos

- `backdoor.ps1`: script principal en PowerShell que implementa la APT.
- `backdoor.bat`: script auxiliar que lanza el `.ps1` de forma oculta.

---

## 🧪 Uso en laboratorio

> ⚠️ **Este script debe usarse únicamente en entornos de pruebas controladas con consentimiento explícito.**

### 1. Simulación manual

1. Copia los archivos a una máquina virtual con Windows.
2. Ejecuta `backdoor.bat` para lanzar la APT de forma silenciosa.
3. Escucha en la IP/puerto configurado (por defecto, 4444).

```bash
nc -lvnp 4444
```

# Ghostlink

Ghostlink es un script en PowerShell que simula una amenaza persistente avanzada (APT) con fines educativos y de concienciación en ciberseguridad. Está diseñado para ser utilizado en entornos controlados como parte de ejercicios Red Team, formación interna o simulaciones de ataques USB.

---

## 🧩 Características

- **Persistencia automática:** mediante claves de registro y tareas programadas.
- **Instalación oculta:** en rutas del sistema poco inspeccionadas.
- **Ejecución silenciosa:** sin mostrar consola ni ventanas al usuario.
- **Control remoto:** mediante conexión TCP (puerto configurable).
- **Desinstalación remota:** con comando `UNINSTALL` o parámetro `-Action uninstall`.
- **Detección y limpieza profunda:** elimina rastros, tareas, archivos y conexiones.

---

## ⚙️ Archivos

- `backdoor.ps1`: script principal en PowerShell que implementa la APT.
- `backdoor.bat`: script auxiliar que lanza el `.ps1` de forma oculta.

---

## 🧪 Uso en laboratorio

> ⚠️ **Este script debe usarse únicamente en entornos de pruebas controladas con consentimiento explícito.**

### 1. Simulación manual

1. Copia los archivos a una máquina virtual con Windows.
2. Ejecuta `backdoor.bat` para lanzar la APT de forma silenciosa.
3. Escucha en la IP/puerto configurado (por defecto, 4444).

```bash
nc -lvnp 4444
```

### 2. Desinstalación remota

Envía el comando `UNINSTALL` por la conexión TCP, o ejecuta:

.\backdoor.ps1 -Action uninstall

## ⚠️ Aviso legal

Este proyecto ha sido desarrollado con **fines exclusivamente educativos y de concienciación en ciberseguridad**. Su uso está destinado únicamente a entornos de laboratorio y simulación controlada.

**El autor no se hace responsable del uso indebido o malintencionado de este código.** El uso no autorizado de este tipo de herramientas puede ser ilegal y está estrictamente prohibido.
