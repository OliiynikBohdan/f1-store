# Вибираємо базовий образ
FROM nginx:alpine

# Копіюємо конфігурацію Nginx
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Копіюємо файли проекту
COPY index.html /usr/share/nginx/html/index.html

# Відкриваємо порт 80
EXPOSE 80

# Запускаємо Nginx
CMD ["nginx", "-g", "daemon off;"]  