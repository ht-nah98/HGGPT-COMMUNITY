Donation Features



By tienanh14098

3 min

Add a reaction
✅ PHẦN 1 — Thiết kế cơ chế HG Coin & Donation (Final Spec)
I. MÔ HÌNH KINH TẾ (ECONOMY MODEL)
1. Loại tiền
Tên: HG Coin

Phạm vi: chỉ dùng cho Community Sharing

Khác biệt hoàn toàn với HGGPT Point (dùng hệ thống rộng toàn nền tảng)

Tỷ lệ quy đổi thưởng tiền mặt (tự động):
1 HG Coin = 100 VNĐ

2. Hai loại số dư
(1) Giving Balance (Cấp)
Nguồn: Admin/Trưởng phòng cấp đầu chu kỳ

Được dùng: ✔ Donate

Reset theo chu kỳ: ✔ Có

Cấp lại mới theo chu kỳ

(2) Earning Balance (Nhận)
Nguồn: Nhận từ người khác donate

Được dùng: ✖ Không donate lại

Dùng để đối soát cuối kỳ

Reset sau khi Stakeholder “confirmed paying” hoặc đầu chu kỳ mới

3. Chu kỳ (Cycle)
Chu kỳ quản lý trong Community đã có sẵn → HG Coin sẽ gắn vào đây:

Chu kỳ có thể bật/tắt tính năng HG Coin

Chu kỳ mới → reset Giving Balance

Chu kỳ mới → reset Earning Balance (sau khi admin xác nhận đã trả thưởng)

Nhưng:
✔ Dữ liệu donate của bài viết vẫn được giữ lại
→ để đánh dấu bài viết chất lượng cao trong lịch sử.

II. CƠ CHẾ DONATION
1. Donate bằng Badge/Huy hiệu
Cố định 6–8 badge toàn hệ thống (do dev quản lý)

Mỗi badge có giá trị HG Coin cố định

Ví dụ:

Badge

Ý nghĩa

Giá trị

✨ Truyền cảm hứng

Ghi nhận chia sẻ hay

5

🤝 Đồng hành

Góp ý hoặc hỗ trợ

8

🚀 Bứt phá

Ý tưởng mới, sáng tạo

12

🏅 Xuất sắc

Bài viết chất lượng cao

20

🔥 Nỗ lực

Tinh thần chia sẻ

10

🌈 Đột phá

Case study quan trọng

25

(Đây là ví dụ — bạn có thể tinh chỉnh tone theo văn hóa HG.)

2. Quy tắc donate
1 user chỉ được donate 1 lần cho 1 bài viết (tránh spam)

Được donate nhiều bài khác nhau

Các icon sẽ hiển thị dạng:

Có màu nếu user đủ coin

Xám/mờ nếu không đủ coin

Khi nhấn donate:

Mở popup chọn badge + xem giá trị coin tương ứng

Confirm → Donate thành công

3. Giao diện donate
UX giống “reaction nâng cấp”
Giống UI “thả tim”, nhưng cảm xúc hơn

Khi hover → hiển thị tooltip giá trị coin

Popup donate
Hiển thị avatar + tên tác giả bài viết

Hiển thị số dư Giving Balance hiện tại

Hiển thị tất cả badge (màu/xám theo coin)

Nút “Gửi huy hiệu”

4. Sau khi donate
Trừ coin từ Giving Balance của người donate

Cộng coin vào Earning Balance của người nhận

Hiển thị:

Badge dưới bài viết

Tên người donate khi hover

Stack badge nếu nhiều người donate cùng loại

Ví dụ hiển thị:



Xuất sắc (x3)
Truyền cảm hứng (x5)
Đồng hành (x2)
III. HIGHLIGHT & XẾP HẠNG
1. Highlight bài viết chất lượng
Bài viết có nhiều donate nhất group → ưu tiên hiển thị trên đầu (nếu admin bật chế độ này)

Có badge “🔥 Bài viết nổi bật trong chu kỳ”

2. Top người dùng nhận donate
Một widget trong sidebar:

Top 1: Avatar + số coin nhận + huy hiệu vàng

Top 2: Avatar + số coin nhận

Top 3: Avatar + số coin nhận

“Xem thêm” → mở bảng xếp hạng đầy đủ

IV. ĐỐI SOÁT (PAYING & RESET)
1. Dashboard dành cho admin
Admin chọn:

Chu kỳ (Cycle)

Group (private group)

Export/excel báo cáo

Hiển thị 2 bảng:

Bảng 1 — Theo User
| User | Tổng Earning | Tổng bài nhận donate | Số huy hiệu nhận | Quy đổi thành tiền |

Bảng 2 — Theo bài viết
| Bài viết | Tác giả | Tổng Earning | Loại huy hiệu | Lịch sử donate |

2. Sau khi trả thưởng
Admin bấm "Đã trả thưởng":

Earning Balance → reset về 0

Log lịch sử được đánh dấu “Paid”

Chu kỳ mới bắt đầu với Giving Balance mới

3. Đặc biệt:
Dù reset số dư nhưng:

Tag donation và badge vẫn hiển thị trong bài viết cũ
→ phục vụ cho “di sản chất lượng”.

V. TRANG CÁ NHÂN — REFRESH
Bạn yêu cầu cải thiện:

Trang cá nhân mới sẽ hiển thị:
Tổng số HG Coin đã nhận trong kỳ

Badge/huy hiệu đã nhận được

Top bài viết có nhiều người donate nhất

Lịch sử donate (người gửi → mình nhận)

Lịch sử donate mình đã gửi

UI tương tự LinkedIn “Activity” + Meta “Badges”.

