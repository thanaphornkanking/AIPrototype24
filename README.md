# AIPrototype24
AI Prototyping 2024 Thanaphorn kanking

# 📚 บันทึกการเรียนวิชา AIPrototype24

## 🗓 รายการคาบเรียน

| ครั้งที่ | วันที่ | หัวข้อที่เรียน | หมายเหตุ |
|----------|----------|----------------|-------------|
| 1  | YYYY-MM-DD | ᴜʙᴜɴᴛᴜ ᴄᴏᴍᴍᴀɴᴅ ʟɪɴᴇ | - |
| 2  | YYYY-MM-DD | ᴠɪʀᴛᴜᴀʟ ᴍᴀᴄʜɪɴᴇ(ᴠᴍ) | - |
| 3  | YYYY-MM-DD | ... | - |

## 📖 เนื้อหาแต่ละคาบ

# 🏫 คาบที่ 1: [ᴜʙᴜɴᴛᴜ ᴄᴏᴍᴍᴀɴᴅ ʟɪɴᴇ]
<details> 
  <summary>ᴜʙᴜɴᴛᴜ ᴄᴏᴍᴍᴀɴᴅ ʟɪɴᴇ </summary>
  
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
## 3. การ copy และการย้าย file/folder
* หลักการ
  ```
  $cp {ที่อยู่ต้นทางของ file/folder ที่ต้องการคัดลอก} {ที่อยู่ปลายทางที่ต้องการที่จะคัดลอก file/folder ไป}
  $mv {ที่อยู่ต้นทางของ file/folder ที่ต้องการย้าย} {ที่อยู่ปลายทางที่ต้องการที่จะย้าย file/folder ไป}
  ```
* Copy file
  ```
  $cp ./filex ~/testfolder1/testfolder1_1/. # ~ กลับไปที่ home ก่อน
  ```
  ```
  # copy file1 in testfolder1 to testfolder1_1_1
  $cp ./file1 ./testfolder1_1/testfolder1_1_1/.
  # cp ที่นี่/ชื่อไฟล์ ที่นี่/เข้าไปที่1_1/เข้าไปที่1_1_1/เอาไว้ตรงนี้
  ```
* Copy and change the file name
  คัดลอกไฟล์ 1 ไปที่ testfolder1_1_1 โดยให้มีชื่อว่า file2
  ```
  $cp ./file1 ./testfolder1_1/testfolder1_1_1/file2
  ```
* Copy folder
  ```
  # copy folder + change folder name แต่เอาไว้ที่เดิม
  $cp -R ./testfolder1_1_1 ./testfolder1_1_2
  ```
* Move file
  ```
  $ mv ./filex ~/testfolder2/. # ~ home
  $ mv ./filex ../../../testfolder2/.
  ```
### ยกเลิกคำสั่ง
> ctrl+c
</details>
---

# 🏫 คาบที่ 2: [ᴠɪʀᴛᴜᴀʟ ᴍᴀᴄʜɪɴᴇ(ᴠᴍ)]
<details> 
  <summary>ᴠɪʀᴛᴜᴀʟ ᴍᴀᴄʜɪɴᴇ(ᴠᴍ) </summary>
  
![VM](https://github.com/thanaphornkanking/AIPrototype24/blob/main/Lecture/VM%20pic.jpg)

 # 1.การสร้าง VM
เข้า Azure -> Education -> VM -> Create a virtual machine
> password: Nat{National ID}_
 # 2. login/logout  VM จาก PC
 ```
 $ssh username@IP #login
 $exit #logout //จบ section
 ```
 # 3. Move file/folder in PC to Cloud and vice versa 
 __ตอนย้ายต้องอยู่ในเครื่องเท่านั้น!!__
* Format
  ```
  $scp {ที่อยู่ต้นทาง} {ที่อยู่ปลายทาง}
  ```
* ส่งไฟล์จากเครื่องเราไปบน Cloud
  ```
  $scp ./xxx nattntn@IP:/xxx/xxx/.
  $scp -r testfolder1/ nattntn@IP:/home/nattntn/. # cp folder in PC to Cloud
  ```
* ดึงไฟล์จาก cloud มาเครื่องเรา
  ```
  $scp nattntn@IP:/xxx/xxx/yyy.py /home/nattntn
  $scp nattntn@IP:/home/yoke/print.py /home/nattntn # move file from folder name york  on nattntn Cloud to PC
  ```
 # 4. Cloud Shell (ใช้ Terminal on Internet)
 > Shell.Azure.com
* ครั้งแรก ssh เข้า VM ก่อน
  ```
   $ssh username@IP #login
   $exit #logout //จบ section
  ```
* Upload file <ต้องอยู่บน shell แล้วค่อย scp to cloud >
  ```
  # 1. upload file on shell
  # 2. scp file to cloud
  $scp rog.png nattntn@IP:/~/. # ย้ายมาhome // ทำบนshell
  ```
  # 5. สร้างเครื่องที่ให้เพื่อนเข้ามาใช้บน Cloud เราร่วมกันได้
  * 1. สร้างเครื่องให้เพื่อน
    ```
    $sudo adduser {ชื่อเครื่อง} #sudo = super user (เจ้าของเครื่อง) do
    # password
    ```
  * 2. ให้เพื่อนลองเข้า Cloud ที่เราสร้าง บน เครื่องเพื่อน
    ```
    $ssh {ชื่อเครื่องที่สร้าง}@IP #IP super user
    $htop # ดูว่าเพื่อนเข้ามายัง
    ```
  * 3. แก้ไข Permission ของเครื่องที่สร้าง
    super user แก้ไขได้
    ```
    $sudo chmod 755 yoke # chmod = change mode // 7 = owner(r|w|x), 5 = group (r|-|x),5 =other (r|-|x)
    ```
</details>

# 🏫 คาบที่ 2: [ᴠɪʀᴛᴜᴀʟ ᴍᴀᴄʜɪɴᴇ(ᴠᴍ)]
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
