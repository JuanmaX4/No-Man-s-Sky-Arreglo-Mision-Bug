# Fix para Cualquier Misión Bugueada en No Man's Sky: "En multitudes estelares"

Bienvenido, viajero. Esta guía te ayudará a resolver cualquier misión atascada o bugueada en *No Man’s Sky*, como puede suceder al cambiar de galaxia, cargar saves antiguos o tras actualizaciones del juego.

👉 Usaremos como ejemplo práctico la misión **"En multitudes estelares" (Atlantid)**, la cual puede quedarse bloqueada sin razón aparente, impidiendo avanzar en la historia.

Este procedimiento te permitirá **completarla manualmente o reiniciarla** usando el editor de partidas **NMSSaveEditor**.

---

## 🧰 Qué necesitas

- PC con Windows (o sistema compatible con Java)
- Tener una partida de No Man's Sky
- [Descargar el editor NMSSaveEditor](https://github.com/goatfungus/NMSSaveEditor)

---

## ✅ PASOS COMPLETOS

### 1️⃣ Descargar el editor

1. Ve a: [https://github.com/goatfungus/NMSSaveEditor](https://github.com/goatfungus/NMSSaveEditor)
2. Haz clic en **"Releases"**
3. Descarga el `.zip` más reciente
4. Extrae el contenido y abre `NMSSaveEditor.jar`

> 💡 *Requiere tener Java instalado*

---

### 2️⃣ IMPORTANTE!!! Hacer copia de seguridad de tu partida SIEMPRE

Antes de tocar nada, guarda tus archivos de partida aquí:

``C:\Usuarios[TU_USUARIO]\AppData\Roaming\HelloGames\NMS\st_[ID_DE_STEAM]``


Haz copia de estos archivos:

- `save.hg`
- `save2.hg`
- `mf_save.hg`
- `mf_save2.hg`

__💾 ¿Que archivo .hg corresponde al tipo de guardado?__

En la carpeta:

save.hg → 🟢 Guardado manual (punto de restablecimiento)

save2.hg → 🔵 Guardado automático

mf_save.hg → Modo multijugador (manual)

mf_save2.hg → Modo multijugador (automático)

![alt text](image.png)

📁 Recomendado: copia y pégalos en el Escritorio.

---

### 3️⃣ Abrir el editor y cargar tu partida

1. Abre `NMSSaveEditor.jar`
2. Ve a `File > Open File/Path`
3. Selecciona `save.hg` o `save2.hg` (el más reciente)
4. Ve a `Edit > Edit Raw JSON`

📸 *Imagen ejemplo:*
![Abrir archivo](ruta_imagen_open.png)

---

### 4️⃣ Buscar la misión bugueada

Una vez en el editor JSON:

- Presiona `Ctrl + F`
- Escribe: `PURPM1`, `PURPM2`, `PURPM3` o `PURPM_BOAT`

Estas misiones son las distintas etapas de "En multitudes estelares".

📸 *Imagen búsqueda:*
![Buscar PURPM1](ruta_imagen_buscar.png)

---

### 5️⃣ Solucionar el bug

#### Opción A: Marcar misión como completada

Modifica:

```json
"Progress": 255



