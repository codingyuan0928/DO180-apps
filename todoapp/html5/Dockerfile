FROM nginx:alpine

# 創建並設置目錄權限
RUN mkdir -p /var/cache/nginx && \
    chown -R nginx:nginx /var/cache/nginx

# 複製靜態文件到默認目錄
COPY . /usr/share/nginx/html

# 暴露 Nginx 服務端口
EXPOSE 80

# 啟動 Nginx
CMD ["nginx", "-g", "daemon off;"]

