# Базовий образ (повна версія, щоб уникнути проблем з бібліотеками)
FROM node:20

# Робоча директорія
WORKDIR /app

# Копіюємо package.json та package-lock.json
COPY package*.json ./

# Встановлюємо залежності (рекомендовано використовувати npm ci)
RUN npm install --legacy-peer-deps

# Копіюємо решту коду
COPY . .

# Відкриваємо порт 3000
EXPOSE 3000

# Запускаємо
CMD ["npm", "start"]
