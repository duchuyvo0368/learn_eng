# Sử dụng image Node.js phiên bản 18 làm base image
FROM node:16

# Thiết lập thư mục làm việc trong container
WORKDIR /frontend

# Sao chép tệp package.json và package-lock.json vào container
COPY package*.json ./

# Cài đặt các dependency của ứng dụng
RUN npm install --force

# Sao chép toàn bộ mã nguồn vào container
COPY . .

# Chạy ứng dụng React khi container khởi động
CMD ["npm", "start"]
