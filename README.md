# RP2040-Klipper
Board này có sẵn bootloader UF2. Giữ nút boot  trên board rồi cắm qua dây USB vào máy tính sẽ nhận luôn ổ flash USB trên Windows. copy file UF2 vào là tự chạy luôn (ổ flash sẽ biến mất luôn ngay sau khi copy file UF2). 

Dùng file klipper.uf2 có đuôi là USBtoSerial nếu dùng dây USB (BTT-PI sẽ nhận là serial)

Dùng file klipper.uf2 có đuôi là CanRx24_Tx25 nếu dùng Canbus. 2 cổng gpio24 và 25 là CanRX và CanTX cắm vào module cantransceiver cho đúng (không được thì đảo chân nhé)

Nguồn dùng 5V (Vbus trên RP2040)

# Đây là software can chứ RP2040 không có can cứng.

    make menuconfig

Dùng software_canbus ![image](https://github.com/user-attachments/assets/a1e73a49-6cfc-4fd9-bc3b-eea2a604c77f)

Dùng USB ![image](https://github.com/user-attachments/assets/8645524a-61b7-4067-9db8-c5be31456ccb)




