# Session 02 - Blockchain Fundamentals

- Student: Nguyễn Ngọc Bảo Khanh
- GitHub: [@khanhnguyeenx-vie](https://github.com/khanhnguyeenx-vie)
- Submitted: 2026-10-27
- Commit: https://github.com/khanhnguyeenx-vie/dev-lock-bootcamp

## 1. Summary

Tìm hiểu cấu trúc block, transaction, ledger và state trong blockchain.

Hiểu cách mạng P2P kết nối các node để chia sẻ và xác thực dữ liệu.

Nắm được quy trình xử lý giao dịch: tạo giao dịch, phát tán lên mạng, xác thực, đưa vào block và xác nhận.

Hiểu cách các block liên kết bằng hash giúp đảm bảo tính toàn vẹn của dữ liệu.


## 2. Topic notes

1. Block và cấu trúc chuỗi: Block gồm Header (hash block trước, timestamp và dữ liệu xác thực) và Body (danh sách giao dịch). Các block liên kết bằng hash, giúp phát hiện việc thay đổi dữ liệu lịch sử.

2. Transaction (Giao dịch): Là yêu cầu chuyển tài sản hoặc dữ liệu trên blockchain, thường chứa thông tin người gửi, người nhận, giá trị, phí và chữ ký số để xác thực quyền thực hiện.

3. Ledger và State:
- Ledger: Lịch sử giao dịch đã được ghi nhận.
- State: Trạng thái hiện tại của hệ thống, như số dư tài khoản, được cập nhật khi giao dịch được thực thi.
4. Node và mạng P2P: Node tham gia lưu trữ, xác minh hoặc truyền tải dữ liệu. Mạng P2P giúp các node trao đổi thông tin mà không phụ thuộc hoàn toàn vào máy chủ trung tâm.

5. Vòng đời giao dịch: Tạo giao dịch → Ký số → Phát tán lên mạng → Chờ trong mempool → Được đưa vào block → Xác minh và thực thi → Đạt mức xác nhận hoặc finality.

6. Blockchain Explorer: Công cụ tra cứu dữ liệu blockchain như giao dịch, block, địa chỉ và trạng thái xác nhận. Ví dụ: Etherscan trên Ethereum.

## 3. Work completed

Tham gia buổi học trên Discord (21/10).

## 4. Evidence

[https://drive.google.com/file/d/1NOOx-4MXPyfaWvNTGV_b_BnMgFPgh2WJ/view?usp=sharing](https://drive.google.com/file/d/18bcTzJdKTLlYu3g-I0_JFWanyhEZzRvB/view?usp=sharing)

## 5. Blockers


## 6. Takeaway

1. Hash (Hàm băm): Là kết quả của hàm băm mật mã, chuyển dữ liệu bất kỳ thành chuỗi có độ dài cố định. Ví dụ, SHA-256 tạo hash 256 bit. Đặc điểm: xác định, nhạy với thay đổi dữ liệu và khó suy ngược dữ liệu gốc. MD5 và SHA-1 không còn an toàn cho mục đích bảo mật mật mã.

2. Ứng dụng của Hash trong Blockchain:
- Liên kết block: Mỗi block chứa hash của block trước, giúp phát hiện dữ liệu bị thay đổi.
- Proof of Work (PoW): Thợ đào thử các giá trị nonce để tìm hash đáp ứng mục tiêu độ khó.
- Địa chỉ ví: Một số blockchain sử dụng hàm băm trong quá trình tạo địa chỉ từ public key; địa chỉ không phải khóa riêng.
- Merkle Tree: Băm các giao dịch theo cấu trúc cây để tạo Merkle Root, hỗ trợ kiểm chứng tính toàn vẹn giao dịch hiệu quả.
