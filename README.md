# AIPrototype24
AI Prototyping 2024 Thanaphorn kanking

# 📚 บันทึกการเรียนวิชา AIPrototype24

## 🗓 รายการคาบเรียน

| ครั้งที่ | วันที่ | หัวข้อที่เรียน | หมายเหตุ |
|----------|----------|----------------|-------------|
| 1  | YYYY-MM-DD | ᴜʙᴜɴᴛᴜ ᴄᴏᴍᴍᴀɴᴅ ʟɪɴᴇ | - |
| 2  | YYYY-MM-DD | หัวข้อต่อไป | - |
| 3  | YYYY-MM-DD | ... | - |

## 📖 เนื้อหาแต่ละคาบ

# 🏫 คาบที่ 1: [ᴜʙᴜɴᴛᴜ ᴄᴏᴍᴍᴀɴᴅ ʟɪɴᴇ]
## Command Line พื้นฐานบน Ubuntu
### 1. คำสั่งพื้นฐาน
* list ทุกๆ file/folder ที่อยู่ใน folder ปัจจุบัน
  ```
  $ls
  ```
  ```
  $ls -{option}
  #ex
  $ls -ltr # บอกรายละเอียดไฟล์
  ```
* ระบุตำแหน่งปัจจุบันที่เราอยู่ในระบบ
  ```
  $pwd
  ```  
### 2. การจัดการ Folder และ File
* create folder
  ```
  $mkdir {foldername}
  ```
* create file 
  ```
  $vi {filename}  # สร้างและเปิดไฟล์ขึ้นมาแก้ไข
  $vi {filename.py} # python file
  #กด i เพื่อแก้ไข
  #กด esc + :wq (ออกแบบ save สิ่งที่เราพิมพ์เข้าไป)
  #กด esc + :q! (ออกแบบไม่ save สิ่งที่อัปลงไป)
  ```
  เวลาจะพิมพ์ กด ***i*** แล้วมันจะขึ้นว่า ***INSERT*** แล้วถึงพิมพ์ได้
  หลังจากนั้นเมื่อพิมพ์เสร็จต้องการที่จะบันทึกให้กด ***esc*** แล้วพิมพ์ **:wq** (write and quit)
* เปิดไฟล์ขึ้นมาดูที่เขียนเฉยๆ
  ```
  $cat {filename}
  ```
* run code Python 
  ```
  $python {filename.py}
  ```
* delete folder
  ```
  $rm -R {foldername}
  ```
* delete file
  ```
  $rm {filename}
  ```
* เปลี่ยนชื่อ file
  ```
  $mv {file เดิม} {file ใหม่}
  $mv ./{file เดิม} ./{file ใหม่}
  # $mv file1 filex # เปลี่ยนชื่อจาก file1 เป็น filex
  ```
* change directory (เข้าไปในfolder)
  ```
  $cd {foldername}
  ```
* ออกจาก folder
  ```
  $cd # home
  $cd ~ # home
  $cd .. # ออกมา 1 step
  $cd ../.. # ออกมา 2 step
  ```
📌 **ตัวอย่างโค้ด:**
```python
print("Hello, World!")
```

---

### 🏫 คาบที่ 2: [หัวข้อที่เรียน]
📅 วันที่: YYYY-MM-DD  
📌 **เนื้อหา:**
- 🔹 จุดที่สำคัญ 1
- 🔹 จุดที่สำคัญ 2
- 🔹 จุดที่สำคัญ 3

📌 **ตัวอย่างโค้ด:**
```python
def add(a, b):
    return a + b

print(add(2, 3))
```

---

✏️ **หมายเหตุ:** สามารถเพิ่มคาบเรียนใหม่ได้โดยคัดลอกโครงสร้างด้านบน และแก้ไขเนื้อหาตามต้องการ
