# 1. Giải pháp kỹ thuật: Thiết lập Files On-Demand

Để laptop 256GB chứa được 500GB dữ liệu mà không bị tràn bộ nhớ, nhóm bắt buộc phải sử dụng tính năng **Files On-Demand (OneDrive)** hoặc **Stream files (Google Drive)**:

- **Cơ chế hoạt động:** Toàn bộ 500GB video sẽ chỉ hiển thị trên máy tính dưới dạng "bóng ma" (Shortcut/Placeholder). Máy tính vẫn nhìn thấy đầy đủ tên file, dung lượng, định dạng nhưng chúng không hề chiếm không gian lưu trữ vật lý trên SSD. Chỉ khi bạn thực sự click đúp để mở một video cụ thể, hệ thống mới bắt đầu tải file đó về.

- **Các bước thiết lập:**
1. Mở phần mềm Google Drive for Desktop (hoặc OneDrive Client) trên máy.
2. Vào **Settings ⚙️** => Chọn chế độ **Stream files** (Truyền phát tệp - đối với Google Drive) hoặc bật **Files On-Demand** (đối với OneDrive).
3. **Quản lý vòng đời dữ liệu:** Sau khi xem hoặc edit xong video đó, click chuột phải vào file => Chọn **Free up space (Giải phóng dung lượng)**. File sẽ lập tức bị xóa khỏi SSD nhưng vẫn nằm an toàn trên Đám mây, trả lại không gian trống cho máy tính.

---

# 2. Báo cáo dung lượng: Chứng minh tính hiệu quả

**Bài toán tài nguyên ban đầu:**
*   Tổng dữ liệu Cloud: **500 GB**
*   Dung lượng ổ SSD Laptop: **256 GB**.

**Kiểm chứng hiệu quả (Sự khác biệt trước và sau):**
*   **❌ Nếu đồng bộ toàn bộ (Mirror files):** 500 GB dữ liệu đổ về > 256 GB trống => Ổ đĩa sẽ báo đỏ tức thì gây tràn bộ nhớ dẫn đến việc bị treo ứng dụng, hệ điều hành Windows crash.
*   **✅ Nếu áp dụng Files On-Demand (Stream files):** 
    *   Dung lượng chiếm dụng để hiển thị toàn bộ cây thư mục 500GB: chỉ tiêu tốn vài MB vì hệ thống chỉ lưu bộ nhớ đệm cho Metadata và Thumbnail.
    *   Làm việc thực tế: Nếu hôm nay bạn cần xử lý 3 video (mỗi video 2GB), bạn mở chúng lên, ổ cứng chỉ tốn **đúng 6 GB** dung lượng cục bộ. Ổ cứng 256 GB dư sức đáp ứng.
    *   Hôm sau, bạn "Free up space" 6 GB đó đi, dung lượng máy tính lại trống trải như mới.
