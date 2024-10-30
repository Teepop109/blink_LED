# ESP32-blink Example - `blink`
blink คือฟังก์ชันสำหรับควบคุมการกระพริบของไฟ LED บนบอร์ด ESP32 โดยทั่วไปโปรแกรมตัวอย่าง "ESP32-blink" จะใช้ในการแสดงวิธีการเปิดและปิด LED เป็นจังหวะ (กระพริบ) เพื่อเป็นพื้นฐานในการเรียนรู้การใช้งาน GPIO (General Purpose Input/Output) ของ ESP32
## ขั้นตอนการใช้งาน
1. เริ่มต้นโดยการเลือกตัวอย่าง `blink`
# ![Screenshot 2024-10-30 204013](https://github.com/user-attachments/assets/6ab7fdb2-87f9-4334-adc1-fe5d772e3c92)

# ![Screenshot 2024-10-30 204020](https://github.com/user-attachments/assets/4c44b34f-0353-417c-ae5d-726295d21c61)


2. หลังจากเลือกตัวอย่างแล้ว ให้กดปุ่ม **Create**
# ![Screenshot 2024-10-30 204026](https://github.com/user-attachments/assets/670fe032-49a2-4536-97ba-50ebdc22777e)


3. ตรวจสอบโค้ดในไฟล์ `main.c`
# ![Screenshot 2024-10-30 204822](https://github.com/user-attachments/assets/33c880f2-2038-4c64-a52a-af452c2350d7)

### การเเก้ไขไฟล์ เพื่อกำหนดขาให้ไฟ LED กระพริบ
# เพิ่มการต่อสายไฟเพื่อใช้งาน

ต่อ LED ตาม GPIO ดังนี้:

| GPIO Pin | LED  |
|----------|------|
| GPIO 18  | LED 1|

# ![Screenshot 2024-10-30 205513](https://github.com/user-attachments/assets/eba9b968-c2e4-4b38-9f96-a4f2b8074ad5)
### หรือการกำหนดตั้งค่า
ไปที่ ESP-IDF: SDK configuration editor (menuconfig) เพื่อตั้งค่าการใช้งานสำหรับโปรเจกต์ blink ตรวจสอบการตั้งค่าในส่วนที่เรียกว่า "Example Configuration" เพื่อกำหนดค่า GPIO
# ![image](https://github.com/user-attachments/assets/5081571b-c21f-4be2-8843-7fb3c5d7d55a)

## ทดสอบ Build และรันโปรแกรม

กด Build และรันโปรแกรม จากนั้นเลือก **UART**

### ผลลัพธ์ที่ได้
ผลลัพธ์จากการรันจะมีลักษณะดังนี้:
# ![Screenshot 2024-10-30 205522](https://github.com/user-attachments/assets/3c98aed5-add9-424d-980c-74019ae86ee2)


ตัวอย่างคลิปวิดีโอ
# [https://drive.google.com/file/d/1NpNbqrlGodH6-1CDzuCmTdsoyTsczfeO/view?usp=sharing](https://drive.google.com/file/d/1XXG5rbf2D7QSyIruq1jWFhhFJzw1hpIm/view?usp=sharing)

### สรุปการทดลอง
BLINK LED สามารถการตั้งค่าและควบคุมการกระพริบของ LED สำหรับ ESP32 ซึ่งปรับใช้งานได้ทั้ง LED GPIO และ addressable LED strip ขึ้นอยู่กับการตั้งค่าของโปรเจกต์เเละความต้องการ
