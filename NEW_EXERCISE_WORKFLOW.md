# Flujo de Trabajo para Añadir un Nuevo Ejercicio de LeetCode

Sigue estos pasos cada vez que quieras añadir la solución a un nuevo problema:

1.  **Asegúrate de estar en el directorio raíz del proyecto:**
    ```bash
    cd /home/leetcode/leetcode
    ```

2.  **Activa el entorno virtual (si no está activo ya):**
    ```bash
    source .venv/bin/activate
    # Tu prompt debería empezar con (.venv)
    ```

3.  **Crea un directorio para el nuevo problema:**
    Usa el número y un nombre descriptivo corto (en minúsculas, con guiones bajos).
    ```bash
    # Ejemplo para el problema 141. Linked List Cycle
    mkdir exercises/141_linked_list_cycle
    ```

4.  **Navega al nuevo directorio:**
    ```bash
    cd exercises/141_linked_list_cycle
    ```

5.  **Crea los archivos necesarios:**
    *   `solution.py`: Aquí irá tu código de Python.
    *   `(Opcional)` `test_solution.py`: Para escribir pruebas unitarias usando `pytest`.
    *   `(Opcional)` `README.md`: Para añadir un enlace al problema, notas sobre tu solución, complejidad, etc.
    ```bash
    touch solution.py
    # touch test_solution.py README.md # Descomenta si los quieres crear
    ```

6.  **Escribe tu código** en `solution.py`.

7.  **(Opcional) Escribe pruebas** en `test_solution.py`.

8.  **Prueba tu solución:**
    *   Puedes ejecutar `python solution.py` si tienes código ejecutable dentro.
    *   Si escribiste pruebas `pytest`:
        ```bash
        # Desde dentro de exercises/141_linked_list_cycle O desde la raíz /home/leetcode/leetcode
        pytest
        # O para ejecutar solo las pruebas de este directorio:
        # pytest .
        ```

9.  **(Opcional) Formatea y verifica tu código:**
    ```bash
    # Formatear con black (ejecutar desde la raíz o el directorio del problema)
    black .
    # Verificar estilo con flake8 o ruff (ejecutar desde la raíz o el directorio del problema)
    flake8 .
    # O
    ruff check . --fix # Ruff puede corregir algunos errores
    ```

10. **Añade los cambios a Git:**
    ```bash
    # Vuelve al directorio raíz
    cd /home/leetcode/leetcode
    # Añade los nuevos archivos
    git add exercises/141_linked_list_cycle/
    # O añade todos los cambios detectados
    # git add .
    # Haz commit con un mensaje descriptivo
    git commit -m "feat: Add solution for 141 Linked List Cycle"
    ```

11. **(Opcional) Sube los cambios si usas un repositorio remoto (GitHub, GitLab...):**
    ```bash
    # git push origin main # O el nombre de tu rama
    ```