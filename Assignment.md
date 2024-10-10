# งาน

## งานที่ 1
![image](https://github.com/user-attachments/assets/59778bfe-0e88-4a53-8991-7ab8731a9f91)

### ตัวอย่าง output ที่คาดหวัง

![image](https://github.com/user-attachments/assets/113c7d7a-2006-4e54-8167-b43f287a018f)




เมื่อกดสวิตช์ จะมีการส่งข้อมูล 0 หรือ 1 ไปยัง mqtt broker
สามารถนำมาพล็อตกราฟดังดังรูป

ผลลัพธ์
![image](https://github.com/user-attachments/assets/25b1886c-0b52-4d29-87b4-2cc970033292)



## งานที่ 2 

เมื่อส่ง topic จาก mqtt explorer มายัง ESP32
จะสามารถควบคุมการติดดับของ LED ได้

ผลลัพธ์
![image](https://github.com/user-attachments/assets/513ae364-b4f6-4a68-9e18-a512eab597c2)
![image](https://github.com/user-attachments/assets/5ab7c487-00c9-4888-80f5-31e2f3620f55)




## งานที่ 3
ส่งตัวเลข 00 - 99 จาก mqtt explorer มายังบอร์ด
แล้วแสดงผลบนตัวเลข 7 ส่วน จำนวนสองหลักบนบอร์ด
โดยใช่ component ที่ดึงมาด้วยไฟล์ idf_component.yml
