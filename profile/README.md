# 🚀 Guía Rápida de Colaboración: SistemasSanNicolas

Bienvenido a la documentación oficial de la organización **SistemasSanNicolas**. Este documento es una guía esencial para estandarizar la forma en que trabajamos y asegurar que el código en `main` sea siempre estable y funcional.

---

## 🛠 La Metodología: GitHub Flow

Para evitar errores ("push a lo wey") y mantener el orden, utilizaremos **GitHub Flow**. La regla de oro es: **Nadie sube cambios directamente a la rama `main`.**

### 1. Configuración de la "Aduana" (Admin únicamente)

Para proteger nuestro trabajo, todos los repositorios deben tener activada la protección de rama:

1. Ve a **Settings > Branches** en el repo de GitHub.

2. Haz clic en **Add branch protection rule**.

3. En *Branch name pattern*, escribe: `main`.

4. Activa las siguientes casillas:

&#x20;  * [x] **Require a pull request before merging**: Obliga a que cada cambio pase por una revisión.

&#x20;  * [x] **Require approvals**: (Recomendado) Al menos una persona debe dar el visto bueno.

---

## 💻 Flujo de Trabajo (Paso a Paso)

Sigue estos 4 pasos siempre que vayas a realizar un cambio, ya seas nuevo o veterano en el equipo:

### Paso 1: Crear una Rama (Branch)

Antes de programar, crea un espacio seguro para tus cambios.

* **En Visual Studio:** Haz clic en `main` (abajo a la derecha) y selecciona **New Branch**.

* **Nombre de la rama:** Usa algo descriptivo (ej: `fix-login`, `mejora-reporte-ventas`, `feature-vistas`).



### Paso 2: Commit y Push

Trabaja en tus archivos normalmente. Al terminar:

1. Haz **Commit** de tus cambios localmente.

2. Haz **Push** hacia el servidor. 

> [!NOTE]

> GitHub te permitirá hacer Push sin problemas porque estás trabajando en **tu propia rama**, no en la principal.



### Paso 3: Crear un Pull Request (PR)

Entra al repositorio en GitHub. Verás un banner amarillo que dice **"Compare \& pull request"**.

* Haz clic ahí para notificar al equipo: *"Oigan, ya terminé mis cambios en esta rama, ¿alguien puede revisarlos para integrarlos a main?"*.



### Paso 4: Revisión y Merge (Fusión)

Aquí es donde ocurre la magia del trabajo en equipo:

1. Un compañero revisa los cambios (el código nuevo sale en verde, lo borrado en rojo).

2. Si hay observaciones, se comentan ahí mismo para corregirlas.

3. Si todo está perfecto, se presiona el botón **Merge pull request**.

4. ¡Felicidades! Tu código ya es parte del proyecto oficial.



---



## ⚠️ Cómo evitar "hacerse bolas" (Conflictos)

Los conflictos ocurren cuando dos personas editan la misma línea al mismo tiempo. Para minimizarlos:



* **Sincroniza siempre:** Antes de empezar el día, haz `Fetch` y `Pull` en tu rama `main` local para tener lo último que subieron los demás.

* **Ramas cortas:** No trabajes en una rama durante semanas. Haz cambios pequeños y súbelos rápido.

* **Comunicación activa:** Si vas a tocar un archivo crítico (ej. `web.config`), avisa en el chat del equipo: *"Voy a mover la config, eviten tocarla unos minutos"*.



---



> **Resumen para el equipo:**

> "Muchachos, nadie le pega al `main` directo. Creen una rama para su tarea, suban sus cambios ahí y abran un Pull Request. Cuando alguien más lo revise y le de 'Merge', el cambio queda oficial."



*Última actualización: 12 de mayo de 2026*

