# 🚀 Guía Paso a Paso: Desplegar en GitHub Pages

## Requisitos Previos
- Tener una cuenta de GitHub (gratis en [github.com](https://github.com))
- Git instalado en tu computadora

---

## PASO 1: Crear Repositorio en GitHub

1. Entra a [github.com](https://github.com) y loguéate
2. Haz clic en el **"+"** en la esquina superior derecha
3. Selecciona **"New repository"**
4. Completa los campos:
   - **Repository name**: `impostor`
   - **Description**: "Impostor - Desafío de Fe | Juego web de fe"
   - **Public** ✓ (debe ser público para GitHub Pages)
   - **Add a README file** ✓
5. Haz clic en **"Create repository"**

---

## PASO 2: Clonar el Repositorio

Abre tu terminal y ejecuta:

```bash
git clone https://github.com/TU_USUARIO/impostor.git
cd impostor
```

**Reemplaza `TU_USUARIO`** con tu nombre de usuario de GitHub.

---

## PASO 3: Agregar los Archivos

1. Copia `index.html` a la carpeta clonada:
   ```bash
   # Si estás en la carpeta del proyecto
   cp /Users/davidcorrea/Documents/code\ projects/impostor/index.html .
   ```

2. Verifica que los archivos estén:
   ```bash
   ls -la
   # Deberías ver:
   # index.html
   # README.md
   # .gitignore
   ```

---

## PASO 4: Subir los Cambios

Ejecuta estos comandos en orden:

```bash
# 1. Agregar archivos
git add index.html README.md .gitignore

# 2. Crear commit
git commit -m "Initial commit: Impostor game"

# 3. Subir a GitHub
git push origin main
```

**Nota**: Si te pide credenciales, usa GitHub CLI o Personal Access Token.

---

## PASO 5: Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings** (Configuración)
3. En el menú izquierdo, busca **"Pages"**
4. Bajo "Build and deployment":
   - **Source**: Selecciona `Deploy from a branch`
   - **Branch**: Selecciona `main` y `/root`
   - Haz clic en **"Save"**

5. Espera 1-2 minutos (GitHub construye el sitio)
6. Verás un mensaje como:
   > "Your site is published at https://TU_USUARIO.github.io/impostor/"

---

## PASO 6: ¡Accede a tu Juego!

Abre tu navegador y ve a:
```
https://TU_USUARIO.github.io/impostor/
```

¡Listo! 🎉

---

## Hacer Cambios Futuros

Si quieres actualizar el juego:

```bash
# 1. Haz cambios en index.html
# 2. Guarda el archivo
# 3. Ejecuta:

git add index.html
git commit -m "Describe tus cambios aquí"
git push origin main
```

Los cambios se reflejarán en 1-2 minutos.

---

## Troubleshooting

### ❌ "Repository not found"
- Verifica que el nombre de usuario sea correcto
- Asegúrate de tener acceso al repositorio

### ❌ Página no aparece
- Espera 2-3 minutos después de push
- Ve a Settings > Pages y verifica la rama correcta
- Comprueba que el repositorio sea **Public**

### ❌ Cambios no se reflejan
- Limpia el caché del navegador (Ctrl+Shift+Del)
- Espera unos minutos, GitHub tarda a veces
- Verifica que el push fue exitoso (`git push` sin errores)

---

## ¡Alternativa Rápida sin GitHub! 

Si prefieres probar localmente primero:

```bash
# En la carpeta del proyecto
cd /Users/davidcorrea/Documents/code\ projects/impostor

# Abre el archivo en tu navegador
open index.html
```

---

¡Ahora a disfrutar! 🎮✨
