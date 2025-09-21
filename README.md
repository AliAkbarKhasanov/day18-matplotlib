# 📊 День 18 — Matplotlib (Базовый)

Учебный модуль из курса **AI & Python**.  
В этом дне мы учимся строить графики и сохранять их в Python с помощью библиотеки **Matplotlib**.  

---

## 🚀 Что изучим
- Линии (одна и несколько на одном поле)  
- Точки (scatter)  
- Столбцы (bar chart)  
- Круговые диаграммы (pie chart)  
- Сохранение графика в файл  

---

## 📂 Структура проекта
day18-matplotlib/
│
├── src/
│ └── day18_matplotlib.py # основной скрипт
│
├── examples/ # PNG картинки (создаются автоматически)
├── docs/
│ └── TELEGRAM_POST.md # пост для Telegram
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore

yaml
Copy code

---

## ⚡ Быстрый старт

1. Клонировать репозиторий:
```bash
git clone https://github.com/AliAkbarKhasanov/day18-matplotlib.git
cd day18-matplotlib
Создать виртуальное окружение и установить зависимости:

bash
Copy code
python -m venv .venv
# Windows
.venv\Scripts\activate
# Linux/Mac
source .venv/bin/activate

pip install -r requirements.txt
Запустить скрипт:

bash
Copy code
python src/day18_matplotlib.py
PNG сохраняются автоматически в папку examples/:

line_plot.png

two_lines.png

scatter.png

bar_chart.png

pie_chart.png

🖼️ Пример графика
Простой линейный график:

python
Copy code
import matplotlib.pyplot as plt

x = [1,2,3,4,5]
y = [2,4,6,8,10]

plt.plot(x, y, label="y = 2x")
plt.title("Простой линейный график")
plt.xlabel("X")
plt.ylabel("Y")
plt.legend()
plt.savefig("line_plot.png")
plt.show()
Результат:



🎯 Домашнее задание
Добавь на график ещё линии: y = x и y = x².

Построй свою столбчатую диаграмму (5–6 категорий).

Измени подписи в круговой диаграмме и сохрани картинку.

🛠 Используемые технологии
Python 3.10+

Matplotlib
