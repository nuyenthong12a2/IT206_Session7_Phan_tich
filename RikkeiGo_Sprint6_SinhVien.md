# Chọn cách dự báo phạm vi cho Sprint 6 (RikkeiGo)

Mình đóng vai Vy (Developer), cùng Lan (Scrum Master) chuẩn bị cho buổi Sprint Planning với Đức (Product Owner).

## Mình tính trước mấy con số

- Velocity 5 Sprint gần nhất: 18, 20, 19, 15, 13.
- **Velocity trung bình** = (18 + 20 + 19 + 15 + 13) / 5 = 85 / 5 = **17 SP**.
- **Khoảng Velocity** (thấp nhất đến cao nhất) là **13 đến 20 SP**.
- Hai Sprint cuối đang giảm (15 rồi 13).
- Capacity Sprint 5 là 212 giờ, Sprint 6 là 186 giờ. 186 / 212 ≈ 0,88 nên Capacity **giảm khoảng 12%** (do Khoa chuyển đi, Minh mới vào chỉ làm khoảng nửa số giờ, Hà nghỉ 3 ngày).

**Xem PBI nào đã sẵn sàng:**

| # | PBI | SP | Đã đủ rõ chưa? | Có giúp Sprint Goal không? |
|---|---|---|---|---|
| 1 | Hẹn giờ đặt xe trước | 5 | Rồi (AC đầy đủ) | Có, khách chủ động đặt trước theo giờ mình muốn |
| 2 | Theo dõi vị trí tài xế | 13 | **Chưa** (thiếu AC khi mất GPS, lại rất lớn) | Có, nhưng chưa làm được |
| 3 | Gửi SMS khi tài xế sắp đến | 3 | Hợp đồng SMS đã ký, nhưng đề **không nói AC đã đủ chưa** | Có, trực tiếp |
| 4 | Chat với tài xế | 5 | Rồi (AC đầy đủ) | Có, khách liên lạc được khi chờ |
| 5 | Giao diện chủ đề Tết | 2 | Rồi (AC đầy đủ) | Không liên quan |

Mình hiểu là PBI chưa đủ rõ thì chưa nên đưa vào Sprint.

---

## Phần 1. Hai cách dự báo

### Cách A: Dựa vào Velocity trung bình

Ý của cách này là: đội trước giờ làm trung bình bao nhiêu thì Sprint này nhận bấy nhiêu, rồi lấy PBI từ trên xuống theo thứ tự Đức xếp.

- Con số dự báo: **17 SP**.
- Danh sách chọn: #1 (5 SP) + #2 (13 SP) = **18 SP**. Gần 17 và vẫn nằm trong khoảng 13 đến 20.

### Cách B: Dựa vào Capacity, Sprint Goal và độ sẵn sàng của PBI

Ý của cách này là: nhìn vào Sprint 6 đội còn bao nhiêu sức, rồi chỉ chọn PBI đã rõ và phục vụ Sprint Goal.

- Mình tính tham khảo: Sprint 5 làm 13 SP, nhân 0,88 thì khoảng 11 SP. Trung bình 17 nhân 0,88 thì khoảng 15 SP. Vậy dự báo khoảng **11 đến 15 SP**.
- Mình biết Capacity giảm 12% không có nghĩa Velocity giảm đúng 12%, nên chỉ dùng phép nhân này làm mốc tham khảo thôi.
- Con số dự báo: **13 SP**.
- Danh sách chọn: #3 (3 SP) + #4 (5 SP) + #1 (5 SP) = **13 SP**. Nếu còn dư sức thì thêm #5 (2 SP).

---

## Phần 2. So sánh hai cách

| Tiêu chí | Cách A: Velocity trung bình | Cách B: Capacity + Sprint Goal + PBI đã rõ |
|---|---|---|
| **Phản ánh thay đổi Capacity** | **(–)** 17 SP là số của 5 Sprint trước, lúc đó chưa có chuyện Khoa đi, Minh mới và Hà nghỉ, nên dễ nhận quá nhiều. | **(+)** Tính từ chính Capacity 186 giờ của Sprint 6, nên có tính đến thay đổi nhân sự. |
| **Bảo vệ Sprint Goal** | **(–)** Lấy theo thứ tự nên dính #2 (13 SP) chưa đủ AC, chiếm khoảng 72% khối lượng. #2 mà không xong thì Sprint Goal hỏng theo. | **(+)** Chọn PBI theo Goal và chỉ lấy cái đã rõ. Có #5 làm phần dự phòng, thêm hay bỏ cũng không ảnh hưởng Goal. |
| **Dễ giải thích với Product Owner** | **(+)** Chỉ có một con số trung bình, dễ nói và dễ hiểu. | **(–)** Phải giải thích nhiều thứ (Capacity, độ rõ của PBI, Goal), và kết quả là một khoảng. Mình khắc phục bằng bảng lý do ở trên. |

---

## Phần 3. Lựa chọn

**Mình chọn Cách B**, vì ba lý do:

1. **Velocity:** 13 SP nằm ở đầu thấp của khoảng 13 đến 20 và bằng đúng Sprint 5, hợp lý khi Velocity đang giảm.
2. **Capacity:** giảm khoảng 12% và có người mới chỉ làm nửa số giờ, nên không nên nhận theo trung bình 17.
3. **Độ rõ của PBI:** #2 chưa đủ AC và quá lớn, chưa nên đưa vào Sprint.

### Sprint Goal đề xuất

> **Khách chủ động hơn khi chờ tài xế: được báo SMS khi tài xế sắp đến, liên lạc được với tài xế qua chat và đặt xe trước theo giờ mong muốn.**

### Danh sách PBI mang vào Sprint Planning

| Thứ tự | PBI | SP |
|---|---|---|
| 1 | Gửi SMS khi tài xế sắp đến | 3 |
| 2 | Chat với tài xế | 5 |
| 3 | Hẹn giờ đặt xe trước | 5 |
| | **Tổng** | **13** |
| Dự phòng | Giao diện chủ đề Tết (làm nếu còn dư, không thuộc Goal) | 2 |

**Mình cần lưu ý:**
- PBI #3 (SMS): đề chỉ nói hợp đồng đã ký, chưa nói AC đã đủ chưa. Mình sẽ hỏi Đức và xác nhận AC trước buổi Planning.
- PBI #2 (theo dõi vị trí) không đưa vào Sprint này. Cần bổ sung AC khi mất GPS và chia nhỏ trong Backlog Refinement.
- 13 SP là dự báo, chốt cuối cùng là do Developers quyết định trong Sprint Planning.
- Velocity giảm hai Sprint liên tiếp thì nên đem ra Retrospective để tìm nguyên nhân, không phải để đổ lỗi cho ai.

### Phản hồi đề nghị 20 SP của quản lý

> Velocity là số điểm đội đã làm xong trong quá khứ để dự báo, không phải chỉ tiêu phải tăng. Nếu bắt đội "đạt số" thì đội sẽ ước lượng cao lên hoặc làm ẩu để đủ điểm, khi đó Velocity không còn đáng tin. Sprint 6 Capacity giảm khoảng 12%, có người mới và người nghỉ phép, lại còn một PBI lớn chưa đủ rõ, nên đội dự báo khoảng 13 SP; 20 SP chỉ bằng Sprint tốt nhất trước đây, nhận lúc này dễ làm không đạt Sprint Goal.
