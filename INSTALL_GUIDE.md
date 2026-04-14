# 🛠️ Hướng dẫn Tích hợp Prime Skills vào Công cụ Coding AI

Bộ kỹ năng **Prime Skills** được thiết kế để hoạt động tốt nhất khi được tích hợp sâu vào quy trình của bạn. Dưới đây là cách cài đặt cho từng công cụ phổ biến:

---

## 1. Sử dụng với Cursor (Khuyên dùng)

Cursor hỗ trợ thư mục quy trình riêng biệt, giúp AI tự động tuân thủ.

### Cách A: Sử dụng `.cursor/rules/` (Tự động)
1. Trong gốc dự án của bạn (Project Root), tạo thư mục: `.cursor/rules/`
2. Copy các file `.md` từ bộ Prime Skills vào thư mục này.
3. Ví dụ: copy `portfolio-craft/SKILL.md` và đặt tên thành `portfolio-craft.md`.
4. **Kết quả**: Khi bạn chat với Cursor hoặc sử dụng Composer, nó sẽ tự động đọc các quy tắc này.

### Cách B: Sử dụng Notepads (Tùy chọn)
1. Mở Cursor -> Settings -> Notepads.
2. Tạo một Notepad mới tên: `Prime-Spec` hoặc `Prime-Portfolio`.
3. Dán nội dung của các file `SKILL.md` tương ứng vào.
4. Khi cần dùng, hãy gõ `@Prime-Spec` trong ô Chat để AI nạp bối cảnh.

---

## 2. Sử dụng với Claude Code (CLI)

Claude Code tìm kiếm các file quy tắc như `CLAUDE.md` hoặc các plugin để hoạt động.

### Bước 1: Cài đặt Plugin (Local)
Nếu bạn có mã nguồn Prime Skills máy, bạn có thể cài đặt như một plugin:
```bash
claude --plugin-dir /đường/dẫn/đến/skills-prime
```

### Bước 2: Sử dụng `CLAUDE.md`
Copy nội dung từ file [CLAUDE.md.template](CLAUDE.md.template) vào file `CLAUDE.md` ở thư mục gốc dự án của bạn. File này sẽ hướng dẫn Claude luôn tuân thủ quy trình Prime (Spec -> Plan -> Build -> Verify).

---

## 3. Sử dụng với Windsurf / VSCode Copilot

### Đối với Windsurf:
1. Tạo hoặc chỉnh sửa file `.windsurfrules` ở gốc dự án.
2. Dán nội dung của các kỹ năng bạn muốn áp dụng vào file này.

### Đối với GitHub Copilot:
1. Tạo file `.github/copilot-instructions.md`.
2. Dán nội dung quy trình Prime Skills vào để Copilot biết cách xử lý các tác vụ phức tạp.

---

## 💡 Mẹo sử dụng hiệu quả

*   **Đừng nạp tất cả cùng lúc**: Mỗi công cụ AI đều có giới hạn bộ nhớ (Context Window). Hãy chỉ nạp 2-3 kỹ năng quan trọng nhất cho tác vụ hiện tại.
*   **Ra lệnh rõ ràng**: Hãy nói: *"Hãy làm theo quy trình `/spec` trong bộ Prime Skills để thiết kế tính năng này"*.
*   **Sử dụng Meta-Dispatcher**: Luôn nạp kỹ năng `prime-orchestrator` đầu tiên để AI có một "người quản lý" biết cách điều phối các kỹ năng khác.

---
*Mọi thắc mắc bạn có thể tham gia thảo luận tại Repo GitHub của mình!*
