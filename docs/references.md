# References

ไฟล์นี้ใช้รวบรวมแหล่งข้อมูลที่มีผลต่อการออกแบบ การเลือกอุปกรณ์ การทดสอบ และการเขียนรายงานของโครงการ Tethering Drone

## วิธีเพิ่มรายการอ้างอิง

เพิ่มแต่ละรายการด้วยรูปแบบต่อไปนี้:

```markdown
### ชื่อเอกสารหรือหน้าเว็บ

- **ประเภท:** Paper / Standard / Datasheet / Manual / Website / Video
- **ผู้จัดทำหรือองค์กร:**
- **ลิงก์:**
- **วันที่เข้าถึง:** YYYY-MM-DD
- **ใช้กับงาน:** เช่น Power Budget, Flight Control หรือ Safety
- **สรุป:** ข้อมูลสำคัญและเหตุผลที่เลือกใช้อ้างอิง
```

การเขียนสรุปสั้น ๆ ว่าแหล่งข้อมูลนั้นนำไปใช้กับการตัดสินใจใด จะมีประโยชน์กว่าการเก็บ URL เพียงอย่างเดียว เพราะ URL อาจเปลี่ยนหรือหายไปในภายหลัง

## Project Documents

- Proposal TEAM-PROJECT 3 - ยังไม่ได้เพิ่มไฟล์ต้นฉบับเข้า repository

## Tethered UAV Research

### An Experimental Tethered UAV-Based Communication System with Continuous Power Supply

- **ประเภท:** Peer-reviewed open-access journal article
- **ผู้แต่ง:** Veronica Rodriguez, Christian Tipantuña, Diego Reinoso, Jorge Carvajal-Rodriguez, Carlos Egas Acosta, Pablo Proaño และ Xavier Hesselbach
- **วารสาร:** Future Internet, 2025, 17(7), Article 273
- **DOI:** https://doi.org/10.3390/fi17070273
- **ลิงก์บทความ:** https://www.mdpi.com/1999-5903/17/7/273
- **วันที่เข้าถึง:** 2026-09-09
- **ใช้กับงาน:** สถาปัตยกรรม Tethered UAV, ระบบจ่ายไฟต่อเนื่องจากภาคพื้นดิน, ground station, การสื่อสาร, การวัดกำลังไฟ และการทดสอบเสถียรภาพที่ความสูง
- **ผลสำคัญ:** ต้นแบบ quadcopter ทำงานอย่างเสถียรที่ 16 V และ 20 A ณ ความสูง 10 เมตร พร้อมให้บริการสื่อสาร VoIP ผ่านอุปกรณ์ Raspberry Pi 4B ด้วย latency ต่ำ งานวิจัยประเมินการใช้พลังงาน เสถียรภาพของ UAV และประสิทธิภาพการส่งข้อมูล
- **ความเกี่ยวข้องกับโครงการ:** เป็นงานอ้างอิงที่ใกล้เคียงโดยตรง เพราะรวมสายจ่ายไฟจาก ground station และระบบสื่อสารบน Tethered UAV สามารถใช้เปรียบเทียบ architecture, power budget และ test methodology ได้ อย่างไรก็ตาม proposal ของโครงการกำหนดระบบส่งกำลังไฟ 48 V จึงไม่ควรนำค่าแรงดันและวงจรจากงานนี้มาใช้โดยตรงโดยไม่มีการคำนวณและทดสอบใหม่
- **ข้อจำกัดที่ควรศึกษา:** ต้นแบบในบทความยังไม่ได้รวมแหล่งจ่ายของ Raspberry Pi เข้ากับ power network หลัก และเสนอ backup battery, ระบบจัดการสายสำหรับความสูงเกิน 10 เมตร และการทดสอบลม/ฝนเป็นงานต่อยอด

### Quadcopter Drone Modeling - MATLAB & Simulink

- **ประเภท:** Technical example / Website / Simulation model
- **ผู้จัดทำหรือองค์กร:** MathWorks
- **ลิงก์หลัก:** https://ww2.mathworks.cn/help/sps/ug/quadcopter-drone.html
- **Source model:** https://github.com/mathworks/Quadcopter-Drone-Model-Simscape
- **วันที่เข้าถึง:** 2026-09-09
- **ใช้กับงาน:** การสร้างแบบจำลองระบบกลไกและไฟฟ้า การประมาณกระแส การควบคุมความสูงและท่าทาง และการทดสอบเสถียรภาพ
- **สรุป:** ตัวอย่างนี้จำลอง quadcopter ด้วย MATLAB, Simulink และ Simscape โดยครอบคลุมมอเตอร์ แบตเตอรี่ โครงสร้างจาก CAD ตัวควบคุม PID แบบ cascade การติดตามเส้นทาง และการทดสอบผลกระทบจากลม เหมาะสำหรับใช้เป็นแนวทางสร้างแบบจำลองและวางแผนการทดสอบของโครงการ แต่ไม่ได้เป็นแบบจำลอง tethered power system โดยตรง จึงต้องพัฒนาส่วนสายโยง ระบบจ่ายไฟ 48 V และวงจรป้องกันเพิ่มเติม

## Power Distribution and Electrical Safety

ยังไม่มีรายการ

## Flight Control and Stability

ยังไม่มีรายการ

## Components and Datasheets

ยังไม่มีรายการ

## Testing and Data Logging

ยังไม่มีรายการ

## Standards and Regulations

ยังไม่มีรายการ

## การเก็บไฟล์อ้างอิง

- เอกสารที่ทีมจัดทำเองและอนุญาตให้เผยแพร่ สามารถเก็บใน `docs/` ได้
- เอกสารภายนอกที่มีลิขสิทธิ์ควรเก็บเป็นลิงก์และข้อมูลบรรณานุกรม ไม่ควรคัดลอกไฟล์เข้า repository
- สำหรับ paper หรือรายงานวิชาการจำนวนมาก สามารถเพิ่มไฟล์ `references.bib` และใช้ Zotero หรือโปรแกรมจัดการบรรณานุกรมในภายหลัง
- ไฟล์ข้อมูลขนาดใหญ่ควรใช้พื้นที่จัดเก็บภายนอก แล้วบันทึกลิงก์ เวอร์ชัน และ checksum ไว้ใน repository
