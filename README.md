# Curso de R — Fundamentos para Análisis de Datos e IA

Este repositorio contiene los **materiales y actividades prácticas** del curso de **R**, orientado a sentar las bases necesarias para trabajar en:

- Análisis Exploratorio de Datos (EDA)
- Estadística aplicada
- Machine Learning clásico
- Flujos de trabajo reales en ciencia de datos

El objetivo principal **no es memorizar sintaxis**, sino **aprender a pensar con datos usando R**.

---

## 🎯 Objetivo del repositorio

Este repositorio tiene dos finalidades claras:

1. **Aprender R desde cero**, entendiendo:
   - variables y tipos de datos
   - operaciones básicas
   - lógica y control de flujo
   - funciones fundamentales
2. **Familiarizarse con un flujo de trabajo profesional**, usando:
   - Jupyter Notebooks
   - Git
   - Pull Requests (PRs)

Las actividades se evaluarán como **Apto / No Apto**.

---

## 📁 Estructura del repositorio

```

.
├─ actividades/        # Notebooks y enunciados oficiales (solo el profesor)
│  └─ Notebook_01.ipynb
│  └─ Notebook_02.ipynb
   └─ ...
│     
│
├─ entregas/           # Entregas de los alumnos (una carpeta por alumno)
│  └─ <apellidos_nombre>/
│     └─ Notebook_01.ipynb
│
└─ README.md

```

⚠️ **Importante**  
- La carpeta `actividades/` **no debe modificarse**
- Cada alumno trabaja **únicamente dentro de su carpeta** en `entregas/`

---

## 🧑‍💻 Cómo trabajar los notebooks

Para cada actividad:

1. Abre el notebook correspondiente en `actividades/`
2. **Copia** el notebook a tu carpeta personal:
```

entregas/<apellidos_nombre>/Notebook_0X.ipynb

```
3. Resuelve los ejercicios directamente en tu copia
4. Ejecuta todas las celdas para comprobar que funciona
5. Antes de entregar:
- Reinicia el kernel
- Limpia los outputs (`Restart & Clear Outputs`)

---

## 🆘 Solución de Problemas: VS Code se queda cargando

Si al intentar abrir el proyecto en un **Dev Container**, Visual Studio Code se queda "atascado" en la pantalla de *Starting Dev Container...* o *Building image...* durante mucho tiempo, sigue estos pasos para construir la imagen manualmente desde la terminal:

1. Abre una terminal (PowerShell, CMD o Bash) en la **carpeta raíz** del proyecto.
2. Ejecuta el siguiente comando para construir la imagen usando el Dockerfile de la carpeta `.devcontainer`:

```bash
docker build -t r-curso -f .devcontainer/Dockerfile .

```

> **Nota:** Asegúrate de incluir el punto `.` al final del comando.

3. Una vez que el proceso termine con éxito (`SUCCESS`), vuelve a Visual Studio Code.
4. Presiona `F1` (o `Ctrl` + `Shift` + `P`) y selecciona:
**Dev Containers: Rebuild and Reopen in Container**.

Al haber construido la imagen manualmente, VS Code la detectará inmediatamente y arrancará sin esperas.

---

## 📤 Procedimiento de entrega (Pull Request)

Las entregas se realizan **exclusivamente mediante Pull Request**.

### Pasos resumidos

Perfecto 👍 Te lo integro dentro del procedimiento completo, adaptado al flujo que quieres que sigan los alumnos.

---

# 📌 Procedimiento para entregar una práctica mediante Pull Request


# 🔧 Procedimiento completo con comandos

## 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/carlostessier/r-fundamentos.git
cd repositorio
```

---

## 2️⃣ Crear una nueva rama para la entrega

⚠️ No trabajar directamente en `main`.

```bash
git checkout -b entrega/apellidos_nombre
```

---

## 3️⃣ Crear la carpeta de entrega

```bash
mkdir -p entregas/apellidos_nombre
```

Coloca dentro:

* `Notebook_01.ipynb` (o el que corresponda)
* Imágenes
* Datasets necesarios
* Cualquier archivo adicional requerido

---

## 4️⃣ Añadir los archivos al control de versiones

```bash
git add entregas/apellidos_nombre/
```

---

## 5️⃣ Hacer commit

```bash
git commit -m "Entrega Notebook 01 - Apellidos Nombre"
```

---

## 6️⃣ Subir la rama al repositorio remoto

```bash
git push -u origin entrega/apellidos_nombre
```

---

## 7️⃣ Crear el Pull Request

Desde la web del repositorio (GitHub/GitLab), crear un PR:

* **Base:** `main`
* **Compare:** `entrega/apellidos_nombre`

O si usas GitHub CLI:

```bash
gh pr create --base main --head entrega/apellidos_nombre --fill
```

---

# 🎯 Buenas prácticas

* No subir datasets muy pesados si no es necesario.
* Comprobar que el notebook ejecuta sin errores antes del commit.
* No modificar archivos de otros compañeros.
* No trabajar nunca directamente sobre `main`.

---

Si quieres, puedo prepararte una versión lista para copiar y pegar en el README del repositorio para los alumnos.


### Reglas de entrega

- ✅ Una carpeta por alumno: `entregas/<usuario_github>/`
- ✅ Un notebook por actividad
- ❌ No modificar archivos fuera de tu carpeta
- ❌ No borrar ni modificar entregas de otros compañeros

Si un Pull Request modifica archivos fuera de tu carpeta, **no se considerará válido**.

---

## ✅ Evaluación

Cada actividad se calificará como:

- **Apto**: la actividad está completa y correctamente resuelta
- **No Apto**: faltan partes, hay errores importantes o no se siguen las normas

---

## 💡 Recomendaciones finales

- Lee los mensajes de error: R explica bastante bien qué falla
- No tengas miedo a equivocarte: cometer errores es parte del aprendizaje
- Prioriza **entender lo que haces**, no solo que “funcione”

---

Si tienes dudas técnicas (Git, Jupyter, R), consúltalas **antes de entregar**.
```

---
