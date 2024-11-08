# Як створити свій перший сайт?

## Що нам буде потрібно для цього:

- [Текстовий редактор](https://notepad-plus-plus.org/)
- [chatgpt](https://chatgpt.com/)
- Браузер

## 📚 Крок 1

Відкрити chatgpt і задати йому наступне питання

> Напиши мені інструкцію з створення найпростішої html сторінки

1. Відкрийте текстовий редактор
2. Створіть новий файл. Збережіть файл з розширенням `.html`. Наприклад, назвіть його `index.html`.
3. Напишіть код HTML

```html
<!DOCTYPE html>
<html lang="uk">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Моя перша сторінка</title>
  </head>
  <body>
    <h1>Привіт, світ!</h1>
  </body>
</html>
```

4. Після того, як ви ввели код, збережіть зміни
5. Відкрийте HTML-файл у браузері

### 🍪 Результат після першого кроку

<img src="https://i.ibb.co/s6L5z1h/Screenshot-2024-11-08-at-22-21-01.png" />

## 📚 Крок 2

> За допомогою html css намалюй в моєму index.html червоне сердечко в центрі сторінки а також підбери красивий фон для всієї сторінки

```html
<!DOCTYPE html>
<html lang="uk">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Червоне сердечко</title>
    <style>
      body {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        margin: 0;
        background: linear-gradient(135deg, #ff9a9e, #fad0c4, #fad0c4, #ff9a9e);
        background-size: cover;
      }

      .heart {
        position: relative;
        width: 30vmin;
        height: 30vmin;
        background-color: red;
        transform: rotate(-45deg);
        display: flex;
        justify-content: center;
        align-items: center;
      }

      .heart::before,
      .heart::after {
        content: "";
        position: absolute;
        width: 30vmin;
        height: 30vmin;
        background-color: red;
        border-radius: 50%;
      }

      .heart::before {
        top: -50%;
        left: 0;
      }

      .heart::after {
        top: 0;
        left: 50%;
      }
    </style>
  </head>
  <body>
    <div class="heart"></div>
  </body>
</html>
```

### 🍪 Результат після другого кроку

<img src="https://i.ibb.co/ynDcghG/Screenshot-2024-11-08-at-22-35-05.png" />

## 📚 Крок 3

> А можеш оновити цей код так щоб сердечко почало пульсувати?

```html
<!DOCTYPE html>
<html lang="uk">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Червоне сердечко</title>
    <style>
      body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
        background: linear-gradient(135deg, #ff9a9e, #fad0c4, #fad0c4, #ff9a9e);
        background-size: cover;
      }

      .heart {
        position: relative;
        width: 30vmin;
        height: 30vmin;
        background-color: red;
        transform: rotate(-45deg);
        display: flex;
        justify-content: center;
        align-items: center;
        animation: pulse 1s infinite;
      }

      .heart::before,
      .heart::after {
        content: "";
        position: absolute;
        width: 30vmin;
        height: 30vmin;
        background-color: red;
        border-radius: 50%;
      }

      .heart::before {
        top: -50%;
        left: 0;
      }

      .heart::after {
        top: 0;
        left: 50%;
      }

      @keyframes pulse {
        0%,
        100% {
          transform: scale(1) rotate(-45deg);
        }
        50% {
          transform: scale(1.1) rotate(-45deg);
        }
      }
    </style>
  </head>
  <body>
    <div class="heart"></div>
  </body>
</html>
```

### 🍪 Результат після третього кроку

[Маленьке сердечко](https://672e7cb2ab98e43ff75f85e1--heart-4b.netlify.app/){:target="\_blank"}
