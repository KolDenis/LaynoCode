# LaynoCode
# Перевірка чи є слово паліндромом

Ця програма на JavaScript перевіряє, чи є введений рядок поліндромом, та виводить відповідний результат.

## Опис

В коді є три функції. Кожна з них, окремо, перевіряє слово чи є воно поліндромом. Чому три? Кожна функція не досконала і може помилятися. Кожна функція перевіряє слово і повертає відповідь. Далі відповіді всіх функцій перевіряється і якщо більше 75% функцій вважають що це поліндром - це поліндром, якщо менше - слово не поліндром.
- Перша функція використвує рекурсивні функції для перевірки паліндрома. Кожна ітерація перевіряє перший та останній символ та обрізає їх. Якщо символи однакові - перехід на іншу ітерацію, якщо ні, слово не є поліндромом. Якщо символів в слові більше нема - це слова поліндром.
- Друга функція використовує стек. Цикл проходиться по кожному символу слова. До середини символи додаються в стек. Далі змінюється направлення, тобто символи починаються видалятися зі стеки порівнюючись з поточними символами ітерації. Якщо на етапі порівняння симаолів буде хоч одна нерівність - слово не поліндром. Якщо ж цикл дійшов до кінця - слово є поліндромом.
- В третій функції реалізована асинхронна перевірка з використанням промісів. Для кожного символа створюється проміс, який з часом поверне значення. Для кожного символа спрацює колбек. Колбек обробляє символ схожим чином, як це реалізовано в другій функції.

## Установка

Для запуску програми вам потрібен Node.js. Ви можете завантажити та встановити його з [офіційного сайту Node.js](https://nodejs.org/).

1. Клонуйте репозиторій на свій комп'ютер:

   ```bash
   git clone https://github.com/KolDenis/LaynoCode.git
   
2. Відкрийте репозиторій
   ```bash
   cd LaynoCode
   
3. Виконайте команду:
     ```bash
   node polindrom.js [ваше слово]
     
