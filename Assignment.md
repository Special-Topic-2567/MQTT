# งาน

## งานที่ 1
![image](https://github.com/user-attachments/assets/59778bfe-0e88-4a53-8991-7ab8731a9f91)

### ตัวอย่าง output ที่คาดหวัง

![image](https://github.com/user-attachments/assets/113c7d7a-2006-4e54-8167-b43f287a018f)


เมื่อกดสวิตช์ จะมีการส่งข้อมูล 0 หรือ 1 ไปยัง mqtt broker
สามารถนำมาพล็อตกราฟดังดังรูป

![image](https://github.com/user-attachments/assets/6f7e3ba7-4f56-446b-9132-d8463282af21)


## งานที่ 2 

เมื่อส่ง topic จาก mqtt explorer มายัง ESP32
จะสามารถควบคุมการติดดับของ LED ได้

![image](https://github.com/user-attachments/assets/398dde87-dee5-4364-96bc-b064fc4da48c)

![image](https://github.com/user-attachments/assets/1ea0fd09-880a-4ff9-9b5f-4bb2f54d2e38)


## งานที่ 3
ส่งตัวเลข 00 - 99 จาก mqtt explorer มายังบอร์ด
แล้วแสดงผลบนตัวเลข 7 ส่วน จำนวนสองหลักบนบอร์ด
โดยใช่ component ที่ดึงมาด้วยไฟล์ idf_component.yml
