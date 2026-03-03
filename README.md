# Домашнє завдання 5 – Методи масивів

## Опис
П'яте домашнє завдання з JavaScript.  
Поглиблена практика роботи з масивами об’єктів, використанням методів масивів у ланцюжках (`map`, `filter`, `sort`, `reduce`, `toSorted` тощо) та стрілочними функціями.

## Технології / стек
- JavaScript (ES6+)
- Стрілочні функції (`=>`)
- Методи масивів:
  - `map()`
  - `filter()`
  - `includes()`
  - `toSorted()` (або `sort()` з поверненням копії)
  - `reduce()`
- Ланцюжки методів (chaining)
- Доступ до вкладених властивостей об’єктів

## Функціонал

| Файл       | Функція                                      | Що робить функція                                                                 |
|------------|----------------------------------------------|------------------------------------------------------------------------------------|
| task-1.js  | `getUserNames(users)`                        | Повертає масив лише імен усіх користувачів (властивість `name`) — використовується `map` |
| task-2.js  | `getUsersWithFriend(users, friendName)`      | Повертає масив користувачів, у яких є друг з іменем `friendName` — використовується `filter` + `includes` |
| task-3.js  | `sortByDescendingFriendCount(users)`         | Повертає користувачів, відсортованих за спаданням кількості друзів — використовується `toSorted` |
| task-4.js  | `getTotalBalanceByGender(users, gender)`     | Повертає сумарний баланс усіх користувачів заданого гендеру — ланцюжок `filter` + `reduce` |

## Приклади роботи (виведення в консоль)

Всі тестові виклики вже присутні в кінці кожного файлу та залишені для перевірки ментором.

Приклади результатів:

- `getUserNames(allUsers)` → `["Moore Hensley", "Sharlene Bush", ..., "Sheree Anthony"]`
- `getUsersWithFriend(allUsers, "Briana Decker")` → масив з Sharlene Bush та Sheree Anthony
- `getUsersWithFriend(allUsers, "Adrian Cross")` → `[]`
- `sortByDescendingFriendCount(users)` → Ross Vazquez перший (3 друзі), Moore Hensley останній (1 друг)
- `getTotalBalanceByGender(clients, "male")` → `12053`
- `getTotalBalanceByGender(clients, "female")` → `8863`

## Демо / деплой

Активне демо доступне за [посиланням](https://artemilliushchenko.github.io/goit-js-hw-05/)

(На сторінці можна побачити результати викликів функцій — або в консолі браузера, або виведені безпосередньо на сторінку.)
