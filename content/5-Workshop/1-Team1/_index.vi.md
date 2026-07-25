---
title: "Team 1 - KFC Ordering Agent"
date: 2026-07-25
weight: 1
---

# Team 1 (First Prize AWS Track)
## Dự án: AI Conversational Ordering Agent for KFC

### ⭐ Key highlight

* Chọn một bài toán rất thực tế: **đặt đồ ăn ngay trong ứng dụng chat** thay vì bắt người dùng cài app.
* Không chỉ trình bày solution mà còn bắt đầu bằng **case study thất bại của McDonald's AI Drive-through**, giúp người nghe hiểu rõ vấn đề trước khi nghe giải pháp.
* Kiến trúc được thiết kế theo hướng **multi-channel**, dễ mở rộng sang các thương hiệu khác ngoài KFC.
* Có phân tích **cost AWS**, latency, scalability chứ không chỉ demo.

---

### 💡 Idea

Xây dựng AI Agent cho phép khách hàng:
* đặt KFC ngay trên Zalo/WhatsApp
* không cần tải app
* AI hiểu hội thoại tự nhiên
* AI tự nhớ lịch sử đặt món
* AI xác nhận đơn hàng trước khi submit để tránh hallucination.

**Workflow:**

```
Chat
↓
Intent Understanding
↓
Planning
↓
Tool Calling
↓
Menu
↓
Promotion
↓
Verify
↓
Order
```

Ngoài ra còn có dashboard để nhân viên theo dõi lịch sử hội thoại nếu AI gặp lỗi.

---

### 📚 Học được gì

#### 1. Pitch nên bắt đầu từ Problem
Không mở đầu bằng architecture. Mở đầu bằng: *"McDonald's từng thất bại vì..."* => người nghe lập tức hiểu pain point. Đây là cách storytelling rất hay.

#### 2. Architecture nên modular
Họ xây:
* Channel Adapter
* Agent Core
* Memory
* Tool
* Dashboard

=> Sau này đổi KFC thành Jollibee chỉ cần thay connector. Đó là mindset của software architecture.

#### 3. Luôn có bước Verify
Họ nhấn mạnh AI không phải lúc nào cũng đúng. Cho nên luôn có:
```
Verify -> Customer confirms -> Submit
```
Đây là cách giảm hallucination cực hay.

#### 4. Cost cũng là một phần của sản phẩm
Họ còn tính: infrastructure cost, latency, Bedrock cost. Điều này làm project có cảm giác rất production-ready.

---

### 💬 Cảm nhận

Đây là bài chia sẻ cân bằng nhất giữa: Business, Technical, Demo, và AWS. Điểm mình thích nhất là họ luôn quay lại "customer experience" thay vì chỉ nói AI mạnh thế nào. Project có tính ứng dụng rất cao.
