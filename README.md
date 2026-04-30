FireLoad Pro — Зональний метод розрахунку пожежі 🔥

[Посилання на калькулятор](https://renderlex.github.io/fire-zone-calculator/)

Калькулятор для моделювання динаміки небезпечних чинників пожежі (НЧП).

---

## 🇺🇦 Українська

### Опис проекту
**FireLoad Pro** — це веб-інструмент для автоматизації складних інженерних розрахунків у сфері пожежної безпеки. Він дозволяє визначити час досягнення гранично допустимих значень (ГДЗ) температури, видимості та концентрації газів у приміщенні з вогнищем та в суміжних задимлених приміщеннях.

### Метод розрахунку
В основі лежить **двозонна (зональна) модель пожежі** згідно з **ДСТУ 8828:2019 (Розділ А.8.4)**.
*   **Математичний апарат:** Система звичайних диференціальних рівнянь (ОДР) балансу маси та енергії.
*   **Чисельний метод:** Інтегрування методом Ейлера з кроком $\Delta t = 0.5$ с.
*   **Газообмін:** Розрахунок витрати диму через прорізи за формулою Бернуллі з урахуванням плавучості.

### Структура та можливості
*   **База даних:** 67 типів пожежних навантажень з довідковими характеристиками.
*   **Динамічна візуалізація:** SVG-схема, що відображає висоту нейтральної площини, температуру та потоки газів у реальному часі.
*   **Інтерактивність:** Додавання необмеженої кількості суміжних приміщень.
*   **Звітність:** Генерація детального звіту з використанням формул KaTeX, готового до друку.

### Мануал
1. Виберіть **Матеріал пожежного навантаження**.
2. Вкажіть параметри **приміщення з вогнищем** ($S, H$).
3. Додайте **суміжні приміщення** та вкажіть розміри прорізів ($b, h$).
4. Натисніть **"Розрахувати"** та перегляньте результати у вкладках.

> **Примітка:** Це тестова версія. Я активно працюю над виправленням помилок та вдосконаленням функціоналу. Критика та пропозиції сприймаються позитивно!

---

## 🇺🇸 English

### Project Description
**FireLoad Pro** is a scientific web tool designed to automate engineering fire safety calculations. It determines the time required to reach critical thresholds for temperature, visibility, and gas concentrations in the fire room and adjacent spaces.

### Methodology
The tool implements the **Two-Zone Fire Model** in accordance with **DSTU 8828:2019 (Section A.8.4)**.
*   **Mathematical Model:** A system of ordinary differential equations (ODEs) for mass and energy balance.
*   **Numerical Method:** Euler integration with a time step of $\Delta t = 0.5$ s.
*   **Gas Exchange:** Calculation of smoke flow through openings ($G_p$) based on Bernoulli's principle with buoyancy effects.

### Key Features
*   **Comprehensive Database:** 67 standardized fire load materials.
*   **Live Visualization:** Dynamic SVG schematic showing smoke layer height, temperature, and gas flows.
*   **Expandability:** Support for multiple adjacent rooms connected via openings.
*   **Professional Reporting:** Detailed calculation breakdowns using KaTeX, optimized for printing.

### Quick Start
1. Select the **Fire Load Material**.
2. Define the **Fire Room** dimensions ($S, H$).
3. Add **Adjacent Rooms** and specify opening sizes ($b, h$).
4. Click **"Calculate All Rooms"** to view hazard dynamics and critical times.

> **Developer Note:** This is a beta version. I am committed to fixing any bugs and improving the tool. Constructive feedback is highly appreciated!
