# Вказуємо базовий образ
FROM python:3.9

# Встановлюємо змінну оточення для непоказу буферизації виводу
ENV PYTHONUNBUFFERED 1

# Створюємо робочу директорію
WORKDIR /app

# Копіюємо requirements.txt у контейнер
COPY requirements.txt /app/

# Встановлюємо залежності
RUN pip install --no-cache-dir -r requirements.txt

# Копіюємо весь код у контейнер
COPY . /app/

# Команда для запуску Django сервісу
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]