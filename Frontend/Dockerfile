FROM nginx:alpine

# ลบไฟล์ default config ของ nginx
RUN rm /etc/nginx/conf.d/default.conf

# คัดลอกไฟล์ HTML และ CSS ของเราไปยัง root directory ของ web server
COPY index.html /usr/share/nginx/html/
COPY style.css /usr/share/nginx/html/

# บอกให้ Container เปิด Port 80
EXPOSE 80

# สั่งให้ nginx เริ่มทำงานเมื่อ container เปิด
CMD ["nginx", "-g", "daemon off;"]