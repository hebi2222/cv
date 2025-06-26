# HebiBot

HebiKoBot là một bot Discord toàn diện, được phát triển với mục đích cung cấp các tính năng quản lý cộng đồng, trò chơi, và hệ thống giao dịch tự động. Bot hỗ trợ nhiều chức năng như mua bán vật phẩm, tham gia trò chơi, và quản lý người dùng thông qua các lệnh Slash (ví dụ: `/shop`, `/use`, `/daily`).

## Mục tiêu

HebiBot được thiết kế để hỗ trợ các cộng đồng Discord trong việc quản lý hoạt động, tương tác với người dùng và cung cấp các trò chơi giải trí. Bot được phát triển bởi Hebi, người chuyên về phát triển bot Discord và các hệ thống tự động hóa.

## Các tính năng chính

- **Quản lý cộng đồng:** Bot cung cấp các lệnh quản lý như `/kick`, `/ban`, `/mute`, `/warn`, giúp người quản trị dễ dàng điều hành server.
- **Trò chơi câu cá:** Người dùng có thể tham gia trò chơi câu cá, nuôi cá và giao dịch các loại cá khác nhau.
- **Hệ thống shop:** Người dùng có thể mua vật phẩm trong shop với các vật phẩm như cần câu, mồi, và các buff hỗ trợ.
- **Nhiệm vụ:** Hệ thống nhiệm vụ giúp người dùng hoàn thành các thử thách và nhận thưởng.
- **Chức năng điểm danh:** Người dùng có thể tham gia điểm danh hàng ngày và nhận thưởng.

## Cài đặt

### Yêu cầu

- Python 3.8 hoặc mới hơn
- Thư viện `discord.py` (hoặc `discord.js` nếu sử dụng JavaScript)
- MongoDB (hoặc cơ sở dữ liệu yêu thích của bạn)
- Các phụ thuộc khác đã được liệt kê trong `requirements.txt`

### Cài đặt dự án

1. **Clone dự án:**

    ```bash
    git clone https://github.com/hebi/hebibot.git
    ```

2. **Cài đặt các phụ thuộc:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Cấu hình bot:**
    - Tạo một bot trên [Discord Developer Portal](https://discord.com/developers/applications).
    - Lấy token bot và đặt vào trong file `config.json`:

    ```json
    {
      "token": "YOUR_BOT_TOKEN"
    }
    ```

4. **Chạy bot:**

    ```bash
    python bot.py
    ```

## Lệnh hỗ trợ

### Quản lý người dùng

- `/kick [user]`: Kicking người dùng khỏi server.
- `/ban [user]`: Cấm người dùng tham gia server.
- `/unban [user]`: Mở khóa người dùng bị cấm.
- `/warn [user]`: Cảnh báo người dùng.

### Trò chơi

- `/fish`: Bắt đầu chơi trò chơi câu cá.
- `/inventory`: Kiểm tra kho cá của bạn.
- `/sell [fish]`: Bán cá cho hệ thống.

### Shop

- `/shop`: Xem danh sách vật phẩm trong shop.
- `/buy [item]`: Mua vật phẩm từ shop.

### Nhiệm vụ

- `/daily`: Nhận phần thưởng hàng ngày.

## Các tệp chính

- **bot.py**: Tệp chính chạy bot.
- **games/fishing.py**: Chứa các logic và dữ liệu trò chơi câu cá.
- **commands.py**: Các lệnh bot được định nghĩa tại đây.
- **config.json**: Cấu hình token và các thông số cần thiết cho bot.

## Đóng góp

Chúng tôi luôn chào đón các đóng góp từ cộng đồng. Nếu bạn muốn đóng góp, hãy fork dự án và tạo pull request với các thay đổi của bạn.

## Liên hệ

Nếu bạn có bất kỳ câu hỏi nào, vui lòng liên hệ với tôi qua email: [hebi.vu220924@gmail.com].

## Giấy phép

Dự án này được cấp phép theo Giấy phép MIT. Vui lòng tham khảo tệp LICENSE để biết chi tiết.

