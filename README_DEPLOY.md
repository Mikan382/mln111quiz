# MLN111 Quiz App v15

Bản v15 tiếp tục từ v14 và sửa trải nghiệm ôn lại câu đã từng trả lời:

- Khi quay lại một câu đã làm, app không tô lại lựa chọn cũ.
- Không hiển thị dòng kiểu `Lần gần nhất làm sai - đã chọn A` trong card câu hỏi.
- Không gắn hint trên đáp án kiểu `Lần trước chọn đáp án này`.
- Lịch sử vẫn lưu để thống kê đúng/sai, nhưng không hiện đáp án từng chọn trên màn hình ôn tập.
- Khi người dùng chọn đáp án trong phiên hiện tại, app vẫn chấm ngay và hiển thị đúng/sai như bình thường.
- Giữ nguyên fix v14: bấm `Tiếp` sau khi trả lời sẽ sang câu tiếp theo, trừ trường hợp câu vừa làm biến mất khỏi bộ lọc hiện tại.

## Deploy Vercel

Framework Preset: Other  
Build Command: `npm run build`  
Output Directory: `dist`

Dữ liệu tiến độ dùng `localStorage`. Nếu deploy cùng domain, app sẽ tự migrate dữ liệu từ các bản cũ.
