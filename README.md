Калькулятор викидів твердих частинок
Опис
Цей веб-калькулятор розроблено для розрахунку валових викидів шкідливих речовин у вигляді суспендованих твердих частинок при спалюванні вугілля, мазуту та природного газу
в енергетичній установці з котлом для факельного спалювання вугілля з рідким шлаковидаленням. Калькулятор базується на методиці, описаній у практичній роботі №2, і використовує
формули та параметри з наданого документа.
Функціональність
Калькулятор дозволяє:

Вводити кількість палива для кожного типу: вугілля (у тоннах), мазуту (у тоннах) та природного газу (у тисячах м³).
Розраховувати показник емісії (k_tb, г/ГДж) та валовий викид (E_tb, тонн) для кожного виду палива.
Виводити загальний валовий викид твердих частинок.
Використовувати параметри, специфічні для:
Вугілля (Донецьке газове ГР): Qr = 20.47 МДж/кг, Ar = 25.20%, a_vin = 0.8, eta_zy = 0.985, Gamma_vin = 1.5%, k_tbS = 0.
Мазуту (Високосірчистий мазут 40): Qr = 39.48 МДж/кг (з урахуванням 2% вологи), Ar = 0.15%, a_vin = 1.0, eta_zy = 0.985, Gamma_vin = 0%, k_tbS = 0.
Природного газу (Уренгой-Ужгород): k_tb = 0, E_tb = 0 (відсутність твердих частинок).


Проводити розрахунки за формулами:
Показник емісії (k_tb):[k_{\text{тв}} = \frac{10^6}{Q_i^r} a_{\text{вин}} \frac{A^r}{100 - \Gamma_{\text{вин}}}(1 - \eta_{\text{зу}}) + k_{\text{твS}}]
Валовий викид (E_tb):[E_{\text{тв}} = 10^{-6} k_{\text{тв}} Q_i^r B]


Перевіряти введені дані (невід’ємні значення) та виводити повідомлення про помилку, якщо не введено жодної кількості палива.

Використання

Відкрийте файл Pz2.html у веб-браузері.
Введіть кількість палива:
Для вугілля: кількість у тоннах.
Для мазуту: кількість у тоннах.
Для природного газу: кількість у тисячах м³.


Натисніть кнопку "Розрахувати викиди", щоб отримати результати.
Перегляньте результати, які включають:
Показник емісії (k_tb, г/ГДж) для кожного виду палива.
Валовий викид (E_tb, тонн) для кожного виду палива.
Загальний валовий викид (тонн).



Технічні деталі

Мова інтерфейсу: Українська.
Технології:
HTML: Структура сторінки.
JavaScript: Логіка розрахунків.
Tailwind CSS: Стилізація для адаптивного та зрозумілого інтерфейсу.


Зовнішні залежності: Tailwind CSS завантажується через CDN (https://cdn.tailwindcss.com).
Формули та параметри: Взяті з документа практичної роботи №2, включаючи таблиці 2.1, А.3, А.4 та контрольний приклад.
Валідація введення: Перевірка на невід’ємні значення та наявність хоча б одного введеного значення палива.
Формат виводу: Результати округлені до двох знаків після коми.

Встановлення

Завантажте файл Pz2.html.
Відкрийте його в будь-якому сучасному веб-браузері (Chrome, Firefox, Safari тощо).
Жодних додаткових залежностей чи серверів не потрібно, оскільки Tailwind CSS завантажується через CDN.

Приклад використання
Вхідні дані:

Вугілля: 1096363 тонн
Мазут: 70945 тонн
Природний газ: 84762 тис. м³

Вихідні дані:

Вугілля:
Показник емісії (k_tb): 150.00 г/ГДж
Валовий викид (E_tb): 3366.00 тонн


Мазут:
Показник емісії (k_tb): 0.57 г/ГДж
Валовий викид (E_tb): 1.60 тонн


Природний газ:
Показник емісії (k_tb): 0.00 г/ГДж
Валовий викид (E_tb): 0.00 тонн


Загальний валовий викид: 3367.60 тонн

Обмеження

Калькулятор не враховує викиди від сорбентів, оскільки в документі вказано, що сіркоочисна установка відсутня (k_tbS = 0).
Природний газ не генерує твердих частинок, тому його викиди завжди дорівнюють нулю.
Параметри (Qr, Ar, a_vin тощо) фіксовані відповідно до документа для конкретних видів палива.
