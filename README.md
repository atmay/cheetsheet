# cheetsheet
Cheetsheet for different tools and technologies

## Cracking the coding interview highlights

- Resizing factor for Python lists depends greatly on the version of CPython but is always more than 1. For some versions it equals to 1.12. 

### Complexity
- Calculating time complexity: 1 + 2 + .... + n equals to n(n+1)/2 or O(n^2)
- Time complexity of .sort() in Python is O(nlogn), it uses Timsort. Timsort is a hybrid stable sorting algorithm, derived from merge sort and insertion sort, designed to perform well on many kinds of real-world data. It was implemented by Tim Peters in 2002 for use in the Python programming language. The algorithm finds subsequences of the data that are already ordered (runs) and uses them to sort the remainder more efficiently. This is done by merging runs until certain criteria are fulfilled. Timsort has been Python's standard sorting algorithm since version 2.3. 

## Alembic

Alembic provides for the creation, management, and invocation of change management scripts for a relational database, using SQLAlchemy as the underlying engine. 

*link: https://alembic.sqlalchemy.org/en/latest/tutorial.html*

- Create migration: `alembic revision -m 'put migration's name here'`

- Apply migration: `alembic upgrade head`

- Rollback latest migration: `alembic downgrade -1`

- See current revision info: `alembic current`

- See full history of revisions: `alembic history --verbose`
