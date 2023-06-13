Руководство по стилю SQL https://www.sqlstyle.guide/ru/

Отформатировать запрос https://codebeautify.org/sqlformatter

Последовательность команд:

`SELECT` 'столбцы или * для выбора всех столбцов; обязательно'

`FROM` 'таблица; обязательно'

`WHERE` 'условие/фильтрация, например, city = 'Moscow'; необязательно'

`GROUP BY` 'столбец, по которому хотим сгруппировать данные; необязательно'

`HAVING` 'условие/фильтрация на уровне сгруппированных данных; необязательно'

`ORDER BY` 'столбец, по которому хотим отсортировать вывод; необязательно'

## Создание таблицы
```sql
CREATE TABLE book (
    book_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(50),
    author VARCHAR(30),
    price DECIMAL(8,2),
    amount INT
);
```

## Вставка записи в таблицу
```sql
INSERT book(title, author, price, amount)
VALUES('Мастер и Маргарита', 'Булгаков М.А.', 670.99, 3);
```
