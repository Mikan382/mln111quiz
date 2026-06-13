# MLN111 Browser Study App - Deploy Vercel

## Cách lưu dữ liệu

App lưu tiến độ ngay trên trình duyệt bằng `localStorage`, gồm:

- Câu đã trả lời
- Câu đúng / sai
- Câu đã đánh dấu
- Lịch sử các lượt trả lời
- Câu đang học dở để vào lại ôn tiếp
- Bộ lọc hiện tại, tab hiện tại, mode hiện tại

Không cần database, không cần server backend.

Lưu ý: localStorage chỉ nằm trên đúng trình duyệt + thiết bị + domain đó. Nếu đổi máy hoặc đổi trình duyệt, dùng nút **Xuất tiến độ** rồi **Nhập tiến độ**.

## Deploy bằng Vercel

Cách 1: Kéo thả folder này lên Vercel.

Cách 2: Push lên GitHub rồi import vào Vercel.

Thông số Vercel:

- Framework Preset: Other
- Build Command: `npm run build`
- Output Directory: `dist`

## Chạy thử local

```bash
npm run start
```

Mở:

```text
http://localhost:3000
```

## File chính

- `index.html`: giao diện
- `style.css`: style xanh nước biển
- `app.js`: logic + dữ liệu câu hỏi + localStorage
- `questions_by_part.json`: dữ liệu tham khảo
- `summary.json`: thống kê bộ câu hỏi
