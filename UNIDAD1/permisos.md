


# Tabla de Permisos de Archivos y Directorios

A continuación se muestra la tabla con los elementos, sus permisos en notación simbólica, octal y una breve descripción basada en la salida del comando `ls -lah`:

| Elemento | Permisos Simbólicos | Permisos Octales | Tipo | Descripción / Significado |
| :--- | :---: | :---: | :---: | :--- |
| **laboratorio-cli** (`.`) | `rwxrwxr-x` | **775** | Directorio | El propietario y el grupo tienen permisos de lectura, escritura y ejecución. Otros tienen lectura y ejecución. |
| **home** (`..`) | `rwxr-x---` | **750** | Directorio | El propietario tiene control total (lectura, escritura, ejecución). El grupo tiene lectura y ejecución. Otros no tienen ningún permiso. |
| **README.txt** | `rw-rw-r--` | **664** | Archivo | El propietario y el grupo pueden leer y modificar el archivo. Otros solo pueden leerlo. |
| **docs** | `rwxrwxr-x` | **775** | Directorio | El propietario y el grupo tienen lectura, escritura y ejecución. Otros solo lectura y ejecución. |
| **logs** | `rwxrwxr-x` | **775** | Directorio | El propietario y el grupo tienen lectura, escritura y ejecución. Otros solo lectura y ejecución. |
| **src** | `rwxrwxr-x` | **775** | Directorio | El propietario y el grupo tienen lectura, escritura y ejecución. Otros solo lectura y ejecución. |

---

### Notas sobre el desglose octal:
* **`7` (`rwx`)**: Lectura (4) + Escritura (2) + Ejecución (1)
* **`6` (`rw-`)**: Lectura (4) + Escritura (2)
* **`5` (`r-x`)**: Lectura (4) + Ejecución (1)
* **`4` (`r--`)**: Lectura (4)
* **`0` (`---`)**: Sin permisos
