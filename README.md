# RIWI Sport – Instrucciones de Uso

## 1. Restaurar la Base de Datos

1. Instala PostgreSQL y crea una base de datos llamada `riwisport`.
2. Restaura el archivo `RiwiSport.sql`:

```sh
psql -U postgres -d riwisport -f RiwiSport.sql
```

## 2. Configurar Variables de Entorno

Crea un archivo `.env` en el mismo directorio que el notebook con el siguiente contenido (ajusta usuario y contraseña):

```
DB_USER=postgres
DB_PASSWORD=Qwe.123*
DB_HOST=localhost
DB_PORT=5432
DB_NAME=riwisport
```

## 3. Instalar Dependencias

Instala los paquetes requeridos:

```sh
pip install pandas numpy sqlalchemy psycopg2-binary matplotlib seaborn python-dotenv
```

## 4. Ejecutar el Notebook

Abre y ejecuta el notebook `analisis_RIWI_Sport_Duana-Ochoa.ipynb` en Jupyter o VS Code.

---

**Dependencias mínimas:**
- pandas
- numpy
- sqlalchemy
- psycopg2-binary
- matplotlib
- seaborn
- python-dotenv

**Nota:** Si cambias los datos de conexión, actualiza el archivo `.env` y el string de conexión en el notebook.
