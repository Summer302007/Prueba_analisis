# RIWI Sport – User Instructions

## 1. Restore the Database

1. Install PostgreSQL and create a database named `riwisport`.  
2. Restore the `RiwiSport.sql` file:

    ```sh
    psql -U postgres -d riwisport -f RiwiSport.sql
    ```

## 2. Set Up Environment Variables

Create a `.env` file in the same directory as the notebook with the following content (adjust the username and password as needed):

```
DB_USER=postgres
DB_PASSWORD=Qwe.123*
DB_HOST=localhost
DB_PORT=5432
DB_NAME=riwisport
```

## 3. Install Dependencies

Install the required packages:

```sh
pip install pandas numpy sqlalchemy psycopg2-binary matplotlib seaborn python-dotenv
```

## 4. Run the Notebook

Open and run the notebook `analisis_RIWI_Sport_Duana-Ochoa.ipynb` in Jupyter or VS Code.

---

**Minimum dependencies:**
- pandas  
- numpy  
- sqlalchemy  
- psycopg2-binary  
- matplotlib  
- seaborn  
- python-dotenv  

**Note:** If you modify the connection details, update both the `.env` file and the connection string inside the notebook.
