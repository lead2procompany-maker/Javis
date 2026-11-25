---
type: wiki
status: active
tags: [wiki, image-guidelines, prompt-engineering, 2pro, studio-standards]
origin: javis-learned
created: 2026-11-20
updated: '2026-11-20'
source: [[conversations/2026-11-20]]
---

# TIÊU CHUẨN HÌNH ẢNH BLOG 2PRO: ĐA DẠNG TRẠNG THÁI, THỰC TẾ VIỆT NAM & ĐỒNG BỘ CAPTION
*(Biên soạn kết hợp cùng Kỹ sư Prompt ảnh & Chuyên gia Hình ảnh Đa dạng)*

Cẩm nang quy chuẩn tạo và kiểm duyệt hình ảnh thương mại cho toàn bộ bài viết blog và sản phẩm trên website 2pro.biz.

---

## 1. NGUYÊN TẮC CỐT LÕI (CORE PRINCIPLES)

1. **BẮT BUỘC DÙNG ẢNH SẢN PHẨM THẬT CỦA 2PRO LÀM THAM CHIẾU (ZERO EXTERNAL IMAGES):**
   - Tuyệt đối KHÔNG tìm kiếm hoặc tải ảnh tham chiếu từ bên ngoài (Google Images, Shopee, Lazada, các trang trôi nổi). Việc này dẫn đến rủi ro nghiêm trọng là AI sinh ra các sản phẩm sai lệch hình dạng, sai màu sắc (như màu tím, hồng) mà 2Pro không hề kinh doanh.
   - BẮT BUỘC lấy ảnh trực tiếp từ kho WooCommerce / WordPress Media Library của 2Pro thông qua Product ID đối chiếu trong kế hoạch bài viết (`aafm-get-post` -> `featured_image.url`).
   - Đưa trực tiếp ảnh gốc của 2Pro vào tham số `images` của công cụ tạo ảnh (Image-to-Image) để AI bảo toàn nguyên vẹn mẫu mã, vật liệu và màu sắc thực tế của 2Pro (khung inox, đầu kẹp xanh ngọc/xanh công nghiệp, lưỡi cao su đen/xám).
2. **Chống bóng nhựa giả tạo AI (Anti-AI Plastic Gloss):** Tránh hiện tượng da người và sàn nhà bóng nhẫy như tượng sáp hoặc đồ họa vi tính 3D rẻ tiền. Dùng ánh sáng tự nhiên khuếch tán (diffused daylight) hoặc đèn studio mềm (softbox 5500K) để tạo độ nhám chân thực của vật liệu inox xước mờ, nhựa nhám ABS và sàn gạch men thực tế.
3. **Chống cứng nhắc & Lặp lại góc chụp**: Tuyệt đối không để sản phẩm trong bài chỉ có duy nhất 1 tư thế đứng thẳng đơ 90 độ ở giữa sàn nhà như hình cắt dán 2D.
4. **Khớp 100% giữa Ảnh và Caption**: Caption bên dưới ảnh chỉ được miêu tả đúng các vật dụng thực tế có trong ảnh. Tuyệt đối không liệt kê các dụng cụ vắng mặt trong hình.
5. **Chân thực văn hóa & Con người Việt Nam (Inclusive & Authentic):** Nhân viên tạp vụ/kỹ thuật mặc trang phục lao động gọn gàng, phù hợp thực tế văn phòng/bệnh viện Việt Nam; vóc dáng và khuôn mặt tự nhiên, không rập khuôn mẫu phương Tây hay tạo hình phi thực tế.
6. **Đa dạng thể loại**: Khuyến khích kết hợp giữa ảnh chụp thực tế và ảnh đồ họa minh họa (infographic, isometric vector, sơ đồ phân vùng).

---

## 2. PHÂN BỔ BỘ 4 HÌNH ẢNH TRONG BÀI BLOG

Mỗi bài blog tiêu chuẩn 3.500 từ bắt buộc có 4 ảnh theo cơ cấu sau:

### Ảnh 1: Ảnh bìa (Cover Banner 800×500 px)
- Bố cục Split-Screen chuẩn 8:5 theo cẩm nang [[cong-thuc-tao-anh-bia-blog-gemini-style]].
- Trái 42% là mảng màu đồ họa tối giản typography (tiêu đề in hoa nổi bật).
- Phải 58% là hình ảnh sản phẩm thực tế trong bối cảnh sử dụng chân thật.

### Ảnh 2: Ảnh Đồ họa Minh họa hoặc Sơ đồ Kỹ thuật (Technical Diagram / Infographic)
- **Mục đích**: Làm rõ cấu tạo, kích thước chi tiết hoặc quy chuẩn phân loại (ví dụ: Sơ đồ thông số kích thước tấm lau 45×15cm, cán inox 135cm; hoặc Infographic phân vùng mã màu 4 khu vực Xanh - Đỏ - Vàng - Trắng).
- **Phong cách**: Đồ họa vector sạch sẽ, nền sáng, chú thích chữ tiếng Việt rõ nét, dễ đọc, mang tính chuyên môn cao.

### Ảnh 3: Ảnh Thao tác Thực tế / Action Shot (Có người thao tác)
- **Mục đích**: Mang lại tính chân thật, sinh động và tăng độ tin cậy E-E-A-T cho người đọc.
- **Bối cảnh**: Nhân viên vệ sinh Việt Nam (mặc đồng phục tạp vụ gọn gàng, đeo găng tay cao su) đang đẩy cây lau trên sàn nhà xưởng epoxy sạch bóng, hoặc đang gạt nước/vắt khăn.
- **Kỹ thuật nhiếp ảnh**: Góc máy ngang thắt lưng (waist-level shot), độ sâu trường ảnh nông nhẹ (shallow depth of field f/2.8 - f/4.0), tiêu cự 50mm tự nhiên, không làm méo hình học không gian.

### Ảnh 4: Ảnh Bố trí Điểm Dụng cụ / Góc Lưu trữ 5S (Storage / Janitor Station)
- **Mục đích**: Hướng dẫn cách bảo quản, cất giữ và tổ chức trạm dụng cụ.
- **Bối cảnh**: Cây lau, chổi, cây gạt nước được xếp đặt chỉn chu trên xe đẩy vệ sinh 3 tầng tại kho đệm hành lang hoặc treo ngay ngắn trên giá 5S.
- **Lưu ý Caption**: Nếu caption viết *"Bộ lau sàn, gạt nước, chổi và hót rác..."* thì ảnh PHẢI có đủ cả 4 món đó trên giá. Nếu ảnh chỉ có cây lau và xô, caption chỉ được viết về cây lau và xô.

---

## 3. CÔNG THỨC PROMPT CHUẨN KỸ SƯ HÌNH ẢNH (PROMPT TEMPLATES)

### Mẫu 1: Action Shot (Nhiếp ảnh thương mại thực tế tại Việt Nam)
> "Chụp ảnh chân thực phong cách commercial photography, kích thước 8:5, tiêu cự 50mm f/3.5, ánh sáng ban ngày tự nhiên qua cửa kính lớn. Một nhân viên vệ sinh nữ người Việt Nam khoảng 35 tuổi, tóc búi gọn gàng, mặc đồng phục tạp vụ màu xanh dương nhạt lịch sự, đeo găng tay cao su vàng, đang thao tác đẩy [tên sản phẩm] trên nền gạch men sáng bóng của sảnh tòa nhà văn phòng hiện đại tại Hà Nội. Góc chụp nghiêng 45 độ tự nhiên, độ tương phản dịu mắt, bối cảnh phía sau mờ nhẹ, không gian sạch sẽ, chuẩn 5S."

### Mẫu 2: Storage Shot (Trạm dụng cụ / Xe đẩy 5S)
> "Chụp ảnh thực tế trạm xe đẩy vệ sinh 3 tầng (Janitor utility cart) chuẩn 5S, kích thước 8:5, góc máy chụp ngang mắt, ánh sáng đèn led trần 5000K sắc nét. Trên xe đẩy bằng nhựa chịu lực màu xám/xanh có: tầng trên đựng khăn lau gấp gọn và bình xịt hóa chất Klenco; bên hông gài gọn gàng 01 cây lau sàn inox cán dài với đầu kẹp xanh ngọc; tầng dưới đặt xô vắt móp đôi màu vàng. Bối cảnh hành lang kho đệm gạch men sạch bong, tường sơn trắng phẳng không có chữ rác."

### Mẫu 3: Infographic / Đồ họa Minh họa
> "Ảnh đồ họa infographic sạch sẽ, chuyên nghiệp, kích thước 8:5, phong cách vector phẳng (flat vector) nền trắng sáng. Minh họa sơ đồ phân loại mã màu dụng cụ vệ sinh theo 4 khu vực chuẩn quốc tế: Xanh dương (khu vực chung), Đỏ (khu vệ sinh rủi ro cao), Vàng (khu sản xuất), Xanh lá (khu căn tin ăn uống). Các biểu tượng sắc nét, chú thích chữ tiếng Việt rõ ràng, bố cục cân đối."

---

## 4. QUY TẮC PHÒNG NGỪA DỊ TẬT SẢN PHẨM, GIẢI PHẪU CON NGƯỜI & CHỮ RÁC AI (ANTI-MUTATION & ANATOMY GUARDRAILS)

### A. Nhận diện các lỗi lộ AI nghiêm trọng cần loại trừ ngay lập tức:
1. **Dị tật giải phẫu con người (Human Anatomical Mutation - LỖI ĐỎ BẮT BUỘC REJECT)**:
   - **Thừa bàn chân / 3 chân**: Dưới một ống quần mọc ra 2 chiếc giày; hoặc một chân chạm sàn bình thường nhưng phía sau gót lại mọc thêm một bàn chân thứ hai đang gác/đạp lên bánh xe đẩy.
   - **Bàn tay dị tật**: Bàn tay dính ngón, thừa ngón (6 ngón), ngón tay cụt hoặc biến dạng như sáp nung chảy.
   - **Khớp xương phi logic**: Cẳng chân hoặc cổ tay bị vặn xoắn 180 độ, tư thế người không có điểm tựa trọng tâm.
2. **Dụng cụ biến dị / "2 đầu"**: Cán cây gạt nước hoặc cây lau bị mọc thêm một đầu gạt nhỏ trên đỉnh chuôi cầm; thân cán đâm xuyên nhau; chổi mọc thêm đầu lau; thanh giằng gãy khúc.
3. **Chữ rác AI (Gibberish Text)**: Ký tự tượng hình méo mó, chữ Cyrillic rác ("СПЕЦМОПОВ") trên biển hiệu hoặc tường.
4. **Dính chùm vật thể**: Quá nhiều dụng cụ chen chúc trên 1 giá treo hẹp dẫn đến việc AI hòa trộn đầu chổi vào cán cây lau hoặc hòa trộn chân người vào bánh xe kim loại.

### B. Bộ quy tắc kỹ thuật khắc phục triệt để:
1. **Nguyên tắc Đơn hành động cho nhân vật (Single-Action Rule)**:
   - Mỗi người trong ảnh CHỈ ĐƯỢC thực hiện duy nhất 01 hành động cơ bản, rõ ràng (ví dụ: *chỉ đẩy xe nhẹ nhàng*, hoặc *chỉ quỳ một gối kiểm tra bánh xe*, hoặc *chỉ dùng tay kéo khay*).
   - TUYỆT ĐỐI CẤM giao 2 hành động đối nghịch cùng lúc (như vừa cúi tay làm việc bên bàn vừa với chân ra sau đạp khóa bánh xe), vì AI Diffusion sẽ phân rã thành 2 nhánh render sinh ra 3 chân.
2. **Quy tắc Kiểm soát Giải phẫu (Anatomy Control)**:
   - Một người CHỈ CÓ ĐÚNG 02 CHÂN và 02 CHIẾC GIÀY.
   - Ưu tiên nhân vật đeo găng tay lao động gọn gàng giúp ngón tay rõ nét.
   - Khoảng cách giữa người và vật dụng kim loại/bánh xe phải có khoảng hở thị giác tối thiểu (không để ống quần dính sát vào bánh xe đẩy).
3. **Ưu tiên Ảnh Tĩnh Sản Phẩm (Still Life) hoặc Cận cảnh thao tác (Close-up Hands)**:
   - Với sản phẩm nhiều thanh kim loại phức tạp (như Giá để ô 120 ngăn, kệ 5S): Ưu tiên chụp tĩnh sản phẩm đặt trang trọng tại góc sảnh (khay nước kéo hờ ra) hoặc chụp cận cảnh đôi tay thao tác, vừa tôn vinh sản phẩm 2Pro vừa triệt tiêu 100% rủi ro dị tật người.
4. **Biển nhãn trơn (Blank Minimalist Signs)**: Yêu cầu biển hiệu gắn tường là bảng trơn không chữ (blank plate) để tránh hoàn toàn chữ rác AI.
5. **Quy trình Vision Audit bắt buộc (Human Anatomy Quality Gate)**:
   - Trước khi upload, agent BẮT BUỘC dùng `javis_describe_image` kiểm tra giải phẫu học: Đếm rõ số chân (=2), số tay (=2), ngón tay (=5). Nếu phát hiện bất kỳ dấu hiệu dị tật nào (`extra foot`, `extra shoe`, `mutated limbs`), BẮT BUỘC REJECT và sinh lại ảnh mới ngay lập tức (tối đa 3 lần).
