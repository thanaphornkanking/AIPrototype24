# AIPrototype2024
Ai Prototyping 2024 Thanaphorn Kanking Student ID: 643021264-9

# 📅 Calendar
|  ᴄʟᴀꜱꜱ  |     ᴅᴀᴛᴇ      |               ᴅᴇꜱᴄʀɪᴘᴛɪᴏɴ                        | 
|:-------:|:-------------:|:-----------------------------------------------:|
|   1     |  DEC 3, 2024  | ᴜʙᴜɴᴛᴜ ᴄᴏᴍᴍᴀɴᴅ ʟɪɴᴇ                         |
|   2     |  DEC 11, 2024 | ᴠɪʀᴛᴜᴀʟ ᴍᴀᴄʜɪɴᴇꜱ                            |
|   3     |  DEC 24, 2024 | ᴄʟᴏᴜᴅ ᴠᴍ                                  |
|   4     |  JAN 7, 2025  | ᴡᴇʙ ᴘᴀɢᴇ                                 |
|   5     |  JAN 21, 2025 | ᴇɴᴠɪʀᴏɴᴍᴇɴᴛ ᴄᴏɴᴅᴀ                         | 
|   6     |  FEB 19, 2025 | ᴡᴇʙ ꜱᴇʀᴠɪᴄᴇ                              |
|   7     |  Mar 11, 2025 | ᴅᴇᴇᴘ ʟᴇᴀʀɴɪɴɢ                             |


# 💼 Contents

<details> 
  <summary> ɢɪᴛʜᴜʙ </summary>
  
* push ขึ้น Git
  ```bash
  git remote add origin <URL ของ repo>       # เพิ่ม remote repository 
  git branch -M main                         # เปลี่ยนชื่อ branch เป็น main (GitHub ใช้ main แทน master)
  git push -u origin main                    # Push โค้ดขึ้น GitHub 
  git config --global user.name "Your Name"  # ตั้งค่าชื่อของผู้ใช้ Git
  git config --global user.email "your-email@example.com"  # ตั้งค่าอีเมลของผู้ใช้ Git
  ```
* คำสั่งใน Github
  ```bash
  git init                             # เริ่มต้น Git repository ใหม่ในโฟลเดอร์ปัจจุบัน
  git status                           # แสดงสถานะของไฟล์ใน repository 
  git branch                           # ตรวจสอบ branch ปัจจุบัน
  git add .                            # เพิ่มไฟล์ทั้งหมดเข้า 
  git commit -m "เพิ่มคำอธิบาย commit"    # บันทึกการเปลี่ยนแปลงใน Git
  git log                              # แสดงประวัติ commit ล่าสุด
  git rm <filename>                    # ลบไฟล์และ commit การลบ
  git mv <old-name> <new-name>         # เปลี่ยนชื่อไฟล์และ commit การเปลี่ยนแปลง
  git push --force                     # บังคับ push ทับของเดิม (ใช้ระวัง)
  ``` 
</details>

<details> 
  <summary> ᴜʙᴜɴᴛᴜ ᴄᴏᴍᴍᴀɴᴅ ʟɪɴᴇ </summary>
  
## 👨🏻‍💻 Command Line พื้นฐานบน Ubuntu
## 1. คำสั่งพื้นฐาน
* list ทุกๆ file/folder ที่อยู่ใน folder ปัจจุบัน
  ```
  $ls
  ```
  ```
  $ls -{option}
  #ex
  $ls -ltr # บอกรายบละเอียดไฟล์
  ```
* ระบุตำแหน่งปัจจุบันที่เราอยู่ในระบบ
  ```
  $pwd
  ```  
## 2. การจัดการ Folder และ File
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
ที่อยู่ของ File/Folder ในตอนสุดท้าย


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
# ยกเลิกคำสั่ง
> ctrl+c

# ขั้นตอนการสร้างไฟล์ด้วย vi

    เข้าสู่โหมดแก้ไข:
        เมื่อเปิดไฟล์ใหม่ขึ้นมาใน vi คุณจะอยู่ในโหมดปกติ (Normal Mode) ซึ่งไม่สามารถพิมพ์ข้อความได้ทันที
        กดปุ่ม i (Insert) เพื่อเข้าสู่โหมดแก้ไข (Insert Mode)

    พิมพ์ข้อความ:
        ตอนนี้คุณสามารถพิมพ์ข้อความในไฟล์ได้ เช่น:

    This is a new file.

บันทึกไฟล์:

    กดปุ่ม Esc เพื่อออกจากโหมดแก้ไข (กลับสู่ Normal Mode)
    พิมพ์ :w แล้วกด Enter เพื่อบันทึกไฟล์

ออกจากโปรแกรม vi:

    หากต้องการบันทึกและออกจากโปรแกรมพร้อมกัน:
        พิมพ์ :wq แล้วกด Enter
    หากต้องการออกโดยไม่บันทึก:
        พิมพ์ :q! แล้วกด Enter

# Homework
copy filex in testfolder1_1 to testfolder1_1_2 and change file name to filey
```
cp ./filex ~/testfolder1/testfolder1_1/testfolder1_1_2/filey
```
</details>


<details> 
  <summary> ᴠɪʀᴛᴜᴀʟ ᴍᴀᴄʜɪɴᴇꜱ </summary>

## 🌐 การใช้งาน Azure Virtual Machines (VM)
Azure Virtual Machines เป็นบริการที่สามารถสร้างเครื่องเสมือน (VM) บนคลาวด์ เพื่อใช้ในการพัฒนาและทดสอบแอปพลิเคชันต่าง ๆ  

### 📌 **1. การสร้าง Virtual Machine บน Azure**
1. เข้าไปที่ **Azure Portal** 👉 [https://portal.azure.com](https://portal.azure.com)
2. ไปที่ **Virtual Machines** > **Create** > **Azure Virtual Machine**
3. กำหนดค่า VM:
   - **Resource group**: สร้างหรือเลือก Resource Group
   - **Virtual Machine Name**: ตั้งชื่อ VM เช่น `tarkung-vm`
   - **Region**: เลือกตำแหน่งเซิร์ฟเวอร์ที่ต้องการ (แนะนำ Southeast Asia)
   - **Image**: เลือก OS เช่น `Ubuntu 20.04 LTS`
   - **Size**: เลือกขนาดของ VM ตามต้องการ
   - **Authentication Type**: 
     - ตั้ง **Username** เช่น `tarkung`
     - ตั้ง **Passwords** เช่น `1234`

4. กด **Review + Create** แล้วกด **Create**
5. รอให้ Azure สร้าง VM เสร็จ จากนั้นไปที่ **Virtual Machines > tarkung-vm** แล้วดู **Public IP Address**

### 🔑 **2. การเข้าใช้งาน Virtual Machine ผ่าน SSH**
เมื่อ VM พร้อมใช้งาน จะสามารถ SSH เข้าไปที่เซิร์ฟเวอร์ได้โดยใช้ IP Address  

#### 🖥 **Linux / macOS / Windows (WSL)**
1. เปิด Terminal หรือ Command Prompt
2. ใช้คำสั่ง SSH เพื่อเข้า VM:
   ```sh
   ssh tarkung@<your-vm-ip>
</details>



<details> 
  <summary> ᴇɴᴠɪʀᴏɴᴍᴇɴᴛ ᴄᴏɴᴅᴀ </summary>

## 🐍 การใช้งาน Conda Environment เบื้องต้น

### 📌 **1. ติดตั้ง Conda**
 Conda สามารถติดตั้งได้จาก:
- **Miniconda** 👉 [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
  #### หรือ
- **Anaconda** 👉 [https://www.anaconda.com/products/distribution](https://www.anaconda.com/products/distribution)

ตรวจสอบว่า Conda ติดตั้งสำเร็จหรือไม่:
```sh
conda --version
```

### 📌 **2. การสร้าง Environment ใหม่**

```sh
conda create --name ai_project python=3.9
```
### 📌 **3. การ Activate และ Deactivate Environment**
การ Activate Environment
```sh
conda activate ai_project
```
การ Deactivate Environment
```sh
conda deactivate
```

### 📌 **4. การลบ Environment**

การ การลบ Environment
```sh
conda remove --name ai_project --all
```
</details>



<details> 
  <summary> ᴡᴇʙ ꜱᴇʀᴠɪᴄᴇ </summary>
  
## 💬 Web Service for Messaging

เป็น Web Service ที่สามารถส่งข้อความระหว่างผู้ใช้ได้ โดยประกอบไปด้วย 2 ส่วนหลัก:

1. **สคริปต์ฝั่งผู้ใช้ (call_web_service.py)**: ช่วยให้ผู้ใช้ป้อนข้อความและเลือกผู้รับเพื่อส่งข้อความ
2. **API ฝั่งเซิร์ฟเวอร์ (firstflask.py)**: รับข้อความจากผู้ใช้ บันทึกรายละเอียด และส่งคำตอบกลับไปยืนยันการรับข้อความ

## ส่วนประกอบ

### 1. สคริปต์ฝั่งผู้ใช้ (`call_web_service.py`)

สคริปต์ฝั่งผู้ใช้จะติดต่อกับ API ฝั่งเซิร์ฟเวอร์เพื่อส่งข้อความ โดยมีขั้นตอนดังนี้:

- ผู้ใช้จะป้อนข้อความที่ต้องการส่ง
- ผู้ใช้สามารถเลือกผู้รับได้ 2 คน: Phu หรือ Ploy
- ส่งข้อความที่เลือกไปยังเซิร์ฟเวอร์ผ่านคำขอ HTTP POST

สคริปต์จะส่งข้อมูลต่อไปนี้ไปยังเซิร์ฟเวอร์:
- `msg`: ข้อความที่ผู้ใช้ป้อน
- `ผู้รับ`: ชื่อของผู้รับข้อความ
- `ip`: ที่อยู่ IP ของผู้รับ
- `ผู้ส่ง`: ชื่อผู้ส่ง

**Code**:
```python
import requests
import json

# URL ของ API
url = 'http://20.255.61.79:5006/simpleAPI'

# ป้อนข้อความจากผู้ใช้
msg = input("กรุณาป้อนข้อความ: ")

# รายชื่อและ IP ที่มีอยู่แล้ว
recipients = {
    "Phu": "104.43.58.161",
    "Ploy": "13.75.95.136"
}

# ให้ผู้ใช้ป้อนชื่อและ IP ของผู้รับเอง หรือเลือกจากที่มีอยู่แล้ว
print("\nเลือกรายชื่อที่ต้องการส่งข้อความ:")
for i, name in enumerate(recipients.keys(), start=1):
    print(f"{i}. {name} (IP: {recipients[name]})")
print(f"{len(recipients) + 1}. ป้อนชื่อและ IP เอง")

choice = input("กรุณาเลือกหมายเลข: ")

if choice.isdigit() and int(choice) in range(1, len(recipients) + 1):
    recipient = list(recipients.keys())[int(choice) - 1]
    ip = recipients[recipient]
else:
    recipient = input("ป้อนชื่อผู้รับ: ")
    ip = input("ป้อน IP ของผู้รับ: ")
    
    # ตรวจสอบว่า IP ซ้ำหรือไม่
    if ip in recipients.values():
        print("\nพบ IP นี้อยู่แล้วในระบบ ข้ามไปยังขั้นตอนถัดไป...")
    else:
        recipients[recipient] = ip  # เพิ่มเข้าไปใน dictionary

# ชื่อผู้ส่ง
sender = "Tarkung"  # สามารถเปลี่ยนเป็น input() เพื่อให้ผู้ใช้ป้อนเองได้

# สร้าง dictionary สำหรับข้อมูลที่จะส่งไป
myobj = {
    'message_key': 'message_val',
    'msg': msg,  # ใช้ข้อความที่ผู้ใช้ป้อน
    'ผู้รับ': recipient,  # ชื่อผู้รับ
    'ip': ip,  # IP ของผู้รับ
    'ผู้ส่ง': sender  # ชื่อผู้ส่ง
}

# แสดงข้อมูลก่อนส่ง
print("\nกำลังส่งข้อความ... \n")
print(f"ข้อมูลที่ส่งไป: ")
print(f"----------------------------")
print(f"ผู้ส่ง: {sender}")
print(f"ผู้รับ: {recipient}")
print(f"IP ของผู้รับ: {ip}")
print(f"ข้อความที่ส่ง: {msg}")
print(f"----------------------------\n")

# ส่งคำขอ POST
x = requests.post(url, data=json.dumps(myobj))

# ตรวจสอบผลลัพธ์และแสดงผล
if x.status_code == 200:
    print(f"การส่งข้อความสำเร็จ! คำตอบจาก API: {x.text}")
else:
    print(f"[ERROR] การส่งข้อความล้มเหลว! รหัสสถานะ: {x.status_code}")
```

</details>

<details> 
  <summary> ᴅᴇᴇᴘ ʟᴇᴀʀɴɪɴɢ </summary>

## Machine learning algorithm ทั่วไป เช่น Linear regression และ logistic regression โครงสร้างการเรียนรู้เป็นดังนี้:
  <div align="center" >
       <img class="RELU"src="https://github.com/thanaphornkanking/AIPrototype24/blob/main/Lecture/deeplearning1.png" style="float: center;" >  
  </div>

  
</details>


# 🏠 Homework
| Homework | Description | Files |
|:--------:|:-----------|:------|
| HW1 | คำนวณจำนวนวันตั้งแต่วันเกิดจนถึงวันปัจจุบัน | `myfirst.py` |
| HW2 | ส่งข้อความด้วย Web Service | `firstflask.py` & `call_web_service.py` |
