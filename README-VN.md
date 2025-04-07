# Seismic Scripts

Kho lưu trữ này chứa một bộ sưu tập các tập lệnh Python được thiết kế để tương tác với **Seismic**, một mạng lưới blockchain hiệu suất cao. Các tập lệnh này cho phép người dùng thực hiện nhiều hành động như nhận token từ hợp đồng token và NFT đã triển khai, đúc token/NFT, gửi giao dịch và quản lý tài sản trên Seismic bằng RPC của mạng. Mỗi tập lệnh được xây dựng bằng thư viện `web3.py` và cung cấp hỗ trợ song ngữ (tiếng Anh và tiếng Việt) để tương tác với người dùng.

Faucet: [Seismic Faucet](https://faucet-2.seismicdev.net/)

## Tổng quan về tính năng

### Tính năng chung

- **Hỗ trợ nhiều tài khoản**: Đọc khóa riêng từ `pvkey.txt` để thực hiện các hành động trên nhiều tài khoản.
- **CLI đầy màu sắc**: Sử dụng `colorama` để có đầu ra hấp dẫn về mặt hình ảnh với văn bản và đường viền có màu.
- **Thực thi không đồng bộ**: Được xây dựng với `asyncio` để tương tác blockchain hiệu quả.
- **Xử lý lỗi**: Bắt lỗi toàn diện cho các giao dịch blockchain và sự cố RPC.
- **Hỗ trợ song ngữ**: Hỗ trợ cả đầu ra tiếng Việt và tiếng Anh dựa trên lựa chọn của người dùng.

### Các tập lệnh được bao gồm

1. **sendtx.py**: Gửi giao dịch token ngẫu nhiên hoặc đến các địa chỉ từ `address.txt` trên Seismic.
2. **deploytoken.py**: Triển khai hợp đồng thông minh token ERC20 trên Seismic.
3. **sendtoken.py**: Gửi token ERC20 đến các địa chỉ ngẫu nhiên hoặc từ `addressERC20.txt` trên Seismic.
4. **nftcollection.py**: Triển khai và quản lý hợp đồng thông minh NFT (Tạo, Đúc, Đốt) trên Seismic.
5. **mintair.py**: Triển khai hợp đồng hẹn giờ trên Seismic.

## Điều kiện tiên quyết

Trước khi chạy tập lệnh, hãy đảm bảo bạn đã cài đặt các phần sau:

- Python 3.8 trở lên
- `pip` (trình quản lý gói Python)
- **Phụ thuộc**: Cài đặt qua `pip install -r requirements.txt` (đảm bảo `web3.py`, `colorama`, `asyncio`, `eth-account`, và `solcx` được bao gồm).
- **pvkey.txt**: Thêm khóa riêng (mỗi dòng một khóa) để tự động hóa ví.
- **address.txt / addressERC20.txt**: Các tệp tùy chọn để chỉ định địa chỉ người nhận.

## Cài đặt

1. **Clone this repository:**
- Mở cmd hoặc Shell, sau đó chạy lệnh:
```sh
git clone https://github.com/thog9/Seismic-testnet.git
```
```sh
cd Seismic-testnet
```
2. **Install Dependencies:**
- Mở cmd hoặc Shell, sau đó chạy lệnh:
```sh
pip install -r requirements.txt
```
3. **Prepare Input Files:**
- Mở `pvkey.txt`: Thêm khóa riêng của bạn (mỗi dòng một khóa) vào thư mục gốc.
```sh
nano pvkey.txt
```
- Mở `address.txt`(tùy chọn): Thêm địa chỉ người nhận (mỗi dòng một khóa) cho `sendtx.py`, `deploytoken.py`, `sendtoken.py`,`nftcollection.py` .
```sh
nano address.txt
```
```sh
nano addressERC20.txt
```
```sh
nano contractERC20.txt
```
```sh
nano contractNFT.txt
```
4. **Run:**
- Mở cmd hoặc Shell, sau đó chạy lệnh:
```sh
python main.py
```
- Chọn ngôn ngữ (Tiếng Việt/Tiếng Anh).

## Liên hệ

- **Telegram**: [thog099](https://t.me/thog099)
- **Channel**: [CHANNEL](https://t.me/thogairdrops)
- **Group**: [GROUP CHAT](https://t.me/thogchats)
- **X**: [Thog](https://x.com/thog099) 

## BUY ME COFFEE

- **BUYMECAFE**: https://buymecafe.vercel.app/
