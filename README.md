# Bank DApp (Sepolia)

เว็บ DApp สำหรับ Assignment 5 เชื่อมต่อ Smart Contract ธนาคารผ่าน MetaMask บน Ethereum Sepolia

## รูปแบบหน้าจอ

- ก่อนใช้งานจะแสดงหน้าเชื่อมต่อ MetaMask ก่อนเข้าสู่หน้าบัญชี
- หน้าจอ desktop ใช้เมนูด้านซ้าย: ภาพรวมบัญชี, ฝากเงิน, ถอนเงิน, ตรวจยอดคงเหลือ และข้อมูลสัญญา
- หน้าจอมือถือใช้เมนูด้านล่าง: ภาพรวม, ฝาก, ถอน และยอดคงเหลือ
- แสดงบัญชีผู้ใช้และข้อมูลนักศึกษาที่กำหนดไว้ในงาน

## ฟังก์ชัน

- เชื่อมต่อ MetaMask และตรวจสอบเครือข่าย Sepolia (Chain ID `11155111`)
- ฝาก Sepolia ETH ด้วย `deposit()`
- ถอน Sepolia ETH ด้วย `withdraw(uint256)`
- ตรวจยอดด้วย `checkBlance()` ตามชื่อที่อยู่ใน Contract
- แสดง Contract Address และลิงก์ไปยัง Sepolia Etherscan

## การเปิดใช้งาน

1. เปิดเว็บผ่านโฮสต์ที่รองรับ HTTPS หรือ local server (เช่น GitHub Pages) ในเบราว์เซอร์ที่ติดตั้ง MetaMask
2. เลือกเครือข่าย Sepolia ใน MetaMask และเชื่อมต่อกระเป๋า
3. ตรวจสอบข้อมูลธุรกรรมใน MetaMask ทุกครั้งก่อนยืนยัน

เว็บนี้โหลด ethers.js v6.17.0 จาก jsDelivr CDN จึงต้องเชื่อมต่ออินเทอร์เน็ตเพื่อใช้งาน Contract

## ข้อมูล Contract

- เครือข่าย: Ethereum Sepolia (Chain ID `11155111`)
- Contract: `0xa8DBCE8522D0A1A5C4C50e9AEF239ed021d00ecA`
- Explorer: <https://sepolia.etherscan.io/address/0xa8DBCE8522D0A1A5C4C50e9AEF239ed021d00ecA>

หน้าเว็บไม่ขอ private key หรือ seed phrase; การยืนยันธุรกรรมทำผ่าน MetaMask
