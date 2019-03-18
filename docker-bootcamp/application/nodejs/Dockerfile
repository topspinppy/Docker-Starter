#กำหนด image เป็น Linux ที่ทำงานอยู่บน Version Apline
FROM node:alpine
#เปลี่ยน dir ไว้ที่ usr app
WORKDIR /usr/app

#Entry Point

COPY ./package.json ./
#copy file [เริ่มต้น] => [สิ้นสุด] เอาไฟล์ทั้งหมดไป
RUN npm install
COPY ./ ./ 
#หลังจาก install แล้วก็จะทำการ เริ่มโปรแกรม
CMD ["npm","start"]



#วิธีรัน 
#
#1. ใช้คำสั่ง docker build . เพื่อ build docker file
#2. ใช้คำสั่ง  docker run -p 3001:3000 [imageid]
#3. docker exec -it [containerid] sh


#ตั้งชื่อ Tag
#                  Repository:NameTag
#docker build . -t mynodeapp:1.0 
#ถ้าไม่ใส่ nametag จะเป็น lastest default


#วิธีรัน
#docker run -p 3004:2222 mynodeapp:1.0
#docker run -p 3002:2222 mynodeapp