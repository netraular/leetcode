# Repositorio de Ejercicios LeetCode en Python

Este repositorio contiene soluciones a problemas de LeetCode implementadas en Python.

## Configuración del Entorno

1.  **Clonar el repositorio (si es necesario):**
    ```bash
    git clone <url-del-repositorio>
    cd leetcode # O el nombre de tu directorio raíz
    ```
2.  **Asegurar la versión de Python (usando pyenv):**
    Este proyecto usa la versión de Python definida en el archivo `.python-version`. Asegúrate de tener `pyenv` instalado y la versión requerida disponible:
    ```bash
    # Instalar la versión si no la tienes (ej. 3.13.0)
    # pyenv install 3.13.0
    # pyenv local 3.13.0 # Normalmente no es necesario si .python-version existe
    ```
3.  **Activar el Entorno Virtual:**
    El entorno virtual (`.venv`) gestiona las dependencias.
    ```bash
    source .venv/bin/activate
    ```
4.  **Instalar Dependencias:**
    ```bash
    pip install -r requirements.txt
    ```

## Estructura de Directorios

*   `.venv/`: Entorno virtual de Python (ignorado por Git).
*   `exercises/`: Contiene las soluciones, organizadas en subdirectorios por problema.
    *   `NNN_nombre_problema/`: Directorio para un problema específico.
        *   `solution.py`: Código de la solución.
        *   `test_solution.py`: (Opcional) Pruebas unitarias con pytest.
        *   `README.md`: (Opcional) Notas específicas del problema, enlace, complejidad.
*   `.gitignore`: Especifica archivos y directorios ignorados por Git.
*   `README.md`: Este archivo.
*   `requirements.txt`: Lista de dependencias de Python.
*   `NEW_EXERCISE_WORKFLOW.md`: Instrucciones para añadir un nuevo ejercicio.

## Ejecutar Pruebas (si usas pytest)

Desde el directorio raíz (`/home/leetcode/leetcode`), después de activar el venv:
```bash
pytest