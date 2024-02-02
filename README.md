# Project-Comor


#Introduction 
    รายงานฉบับนี้เป็นส่วนหนึ่งของวิชา 06016412 COMPUTER ORGANIZATION AND OPERATING SYSTEM ชั้นปีที่2 (2/2023) โดยมีจุดประสงค์เพื่อศึกษาความรู้ที่ได้จากเรื่อง Process ของ Linux ซึ่งรายงานนี้นำเสนอความรู้พื้นฐานเกี่ยวกับProcess ใน Linux โดยอธิบายองค์ประกอบสำคัญของโพรเซส เช่น สถานะprocess การจัดการหน่วยความจำ และการจัดตารางเวลา รวมถึงการทำงานของprocessใน Linux เป้าหมายของรายงานนี้ คือ เพื่อช่วยให้ผู้อ่านเข้าใจระบบprocess ใน Linux และสามารถจัดการprocessต่างๆ บนคอมพิวเตอร์ได้อย่างมีประสิทธิภาพ
    ผู้จัดทำได้เลือกหัวข้อนี้ในการทำรายงาน เนื่องมาจากเป็นเรื่องที่น่าสนใจผู้จัดทำหวังว่ารายงานฉบับนี้จะให้ความรู้ และเป็นประโยชน์แก่ผู้อ่านทุก ๆ ท่าน

#Overview
    ในระบบปฏิบัติการ Linux,  Process ใน Linux คือ เปรียบเสมือนโปรแกรมที่กำลังทำงานอยู่ เป็นหน่วยพื้นฐานของการประมวลผลในระบบ Linux แต่ละ process จะมีหน่วยความจำ พื้นที่ว่างบนดิสก์ และทรัพยากรระบบอื่นๆ ของตัวเอง ช่วยให้ผู้ใช้สามารถทำงานหลายอย่างพร้อมกัน ใช้ทรัพยากรอย่างมีประสิทธิภาพ และปรับแต่งระบบ Linux ให้ทำงานตามต้องการ

ลักษณะสำคัญของ Process:
- มีเอกลักษณ์: แต่ละ process จะมี PID (Process ID) ที่ไม่ซ้ำกัน
- มีสถานะ: Process มีสถานะต่างๆ เช่น รัน (Running), รอ (Waiting), หยุด (Stopped)
- มีลำดับความสำคัญ: Process แต่ละ process จะมีลำดับความสำคัญที่กำหนดว่า process ใดควรได้รับทรัพยากรระบบก่อน
- มีทรัพยากร: Process แต่ละ process จะมีหน่วยความจำ พื้นที่ว่างบนดิสก์ และทรัพยากรระบบอื่นๆ ของตัวเอง
- มีอิสระ: Process แต่ละ process ทำงานแยกกัน ไม่รบกวนกัน

ประเภทของ Process:
- Foreground process: Process ที่ผู้ใช้กำลังโต้ตอบอยู่
- Background process: Process ที่ทำงานอยู่เบื้องหลัง ไม่ได้โต้ตอบกับผู้ใช้
- Daemon: Process ที่ทำงานอยู่เบื้องหลัง โดยปกติจะเริ่มต้นเมื่อระบบบูต และทำงานต่อไปจนกว่าระบบจะปิด

ความสำคัญของ Process:
- การทำงานหลายอย่างพร้อมกัน: Process ช่วยให้ผู้ใช้สามารถทำงานหลายอย่างพร้อมกันบนระบบ Linux
- การใช้ทรัพยากรอย่างมีประสิทธิภาพ: Process ช่วยให้ระบบ Linux สามารถใช้ทรัพยากรระบบอย่างมีประสิทธิภาพ
- การปรับแต่งระบบ: Process ช่วยให้ผู้ใช้สามารถปรับแต่งระบบ Linux ให้ทำงานตามต้องการ

