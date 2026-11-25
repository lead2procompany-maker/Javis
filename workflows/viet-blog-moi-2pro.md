---
type: workflow
name: Viết blog mới 2Pro
slug: viet-blog-moi-2pro
status: active
group: Marketing
description: "Quy trình 5 bước chuyên sâu 2Pro: Chuyên gia SEO hoạch định Topic Cluster & chống ăn thịt từ khóa -> Nghiên cứu từ khóa & lập dàn ý chi tiết -> Biên tập bài viết AIO/GEO & tạo ảnh bìa -> Đăng nháp WordPress với Rank Math tối ưu -> Báo cáo tự động vào Google Sheet theo dõi tiến độ."
steps:
- agent: agency-marketing-seo-specialist
  task: |
    Yêu cầu gốc: {{input}}
    (LƯU Ý QUAN TRỌNG: Đây là bài viết MỚI độc lập. Tuyệt đối KHÔNG sửa bài cũ 22301. Nếu input không có chủ đề cụ thể hoặc để trống, tự động chọn 01 chủ đề mới tiềm năng từ các ngành hàng chủ lực của 2Pro).

    MỤC TIÊU: Hoàn thành nhanh Chiến lược Cụm Chủ Đề (Topic Cluster) & Rà soát Chống Ăn Thịt Từ Khóa (Cannibalization) trong tối đa 1 lượt phân tích, cô đọng dưới 500 từ để bàn giao sang Bước 2:

    CƠ CHẾ ƯU TIÊN KẾ HOẠCH NỘI DUNG (CONTENT PIPELINE FAST-TRACK - TIẾT KIỆM 70% THỜI GIAN & TOKEN):
    - Đọc file Kế hoạch nội dung đã khóa tại `D:\Javis OS\brains\2Pro SEO\work\content-pipeline-2pro.md` (hoặc GitHub `plans/content-pipeline-2pro.md`).
    - Nếu có đề tài mang trạng thái `Pending` và người dùng không yêu cầu chủ đề riêng biệt:
      + LẤY NGAY ĐỀ TÀI ĐÓ RA XỬ LÝ. BỎ QUA HOÀN TOÀN BƯỚC CÀO DỮ LIỆU GSC RƯỜM RÀ.
      + Kế thừa 100% Từ khóa chính, Dàn 7-8 từ khóa phụ, Tiêu đề H1 và Sản phẩm 2Pro đối chiếu đã nghiên cứu sẵn.
      + Xuất nhanh bản tóm lược để chuyển thẳng sang bước Biên tập bài viết!

    1. RÀ SOÁT CHỐNG ĂN THỊT TỪ KHÓA:
       - Xác định rõ Search Intent của bài blog là Informational (Tư vấn, hướng dẫn, so sánh kỹ thuật, tiêu chí lựa chọn).
       - Khẳng định bài blog KHÔNG cướp từ khóa bán hàng ngắn của các trang sản phẩm/danh mục 2Pro.

    2. KHUNG TOPIC CLUSTER & PILLAR LINK:
       - Chọn 01 Pillar Page tương ứng trên 2pro.biz để bài blog trỏ về (ví dụ: Dụng cụ vệ sinh, Hộp đựng xà phòng, Hộp đựng giấy, Thảm sàn, Giấy Sống Vàng, Hóa chất công nghiệp, Bảo hộ lao động).
       - Nêu 3-5 anchor text chiến lược tự nhiên dẫn về danh mục/sản phẩm mục tiêu.

    3. ĐỊNH HƯỚNG ANSWER BOX:
       - Soạn 01 đoạn tóm tắt định nghĩa/giải pháp (40-60 từ) ngay đầu bài để kích hoạt Google AI Overviews / Featured Snippets.
       - Bàn giao ngay bản chiến lược Topic Cluster ngắn gọn sang Bước 2 (Phân tích cơ hội SEO) để lên dàn ý chi tiết.

- agent: phan-tich-co-hoi-seo-2pro
  task: |
    Yêu cầu gốc: {{input}}
    Bản chiến lược Topic Cluster & Chống ăn thịt từ khóa từ Chuyên gia SEO (Bước 1):
    {{prev}}

    MỤC TIÊU: Kế thừa chiến lược Topic Cluster từ Bước 1, nghiên cứu từ khóa chi tiết & lập dàn ý SEO chuyên sâu cho 01 bài blog mới trên 2pro.biz (hoặc cập nhật nếu có chỉ định rõ ID/URL).

    1. QUY CHẾ NGHIÊN CỨU TỪ KHÓA TỰ ĐỘNG (ĐA NGUỒN DỮ LIỆU - JAVIS TỰ ĐỘNG KHAI THÁC):
       - TỰ ĐỘNG TỔNG HỢP TOÀN DIỆN: Javis phối hợp đa nguồn dữ liệu để nghiên cứu từ khóa và phân tích đối thủ cạnh tranh. Người dùng KHÔNG cần phải nhập thủ công nếu chỉ đưa ra chủ đề hoặc để trống.
       - NGUỒN 1 - SEMRUSH & KEYWORD EXPLORER (DASHBOARD TOOL): Tự động quét và đọc các file CSV nghiên cứu từ khóa, Keyword Gap, phân tích đối thủ (như Hanhtinhxanh, Lan Anh, Bich Ha...) trong thư mục Downloads (`~/Downloads`). Đây là nguồn dữ liệu chuyên sâu hàng đầu để tìm khoảng trống từ khóa (Content Gap), xu hướng đối thủ và Search Volume chuẩn xác.
       - NGUỒN 2 - GOOGLE SEARCH CONSOLE: Tự động truy vấn GSC của `sc-domain:2pro.biz` để tìm các truy vấn thực tế có impression, CTR thấp hoặc vị trí 4-20 liên quan đến chủ đề để khai thác kéo rank.
       - NGUỒN 3 - GOOGLE SEARCH SUGGESTIONS & SERP (VIỆT NAM): Tự động tìm kiếm các gợi ý thời gian thực từ Google Việt Nam cho các biến thể long-tail ("cách chọn...", "tiêu chuẩn chọn...", "kinh nghiệm...", "loại nào tốt...", "so sánh...").
       - NGUỒN 4 - AIKTP KEYWORD PLANNER & KHO TRI THỨC: Đối soát Search Volume, Keyword Difficulty và chùm từ khóa LSI từ AIKTP / thư mục `knowledge/keywords`.
       - TỰ ĐỘNG CHỐT BỘ TỪ KHÓA CHUẨN:
         + 01 Primary Keyword (slug <= 40 ký tự, intent Thông tin / Hướng dẫn / Giải pháp B2B).
         + 7-8 Secondary Keywords (từ khóa phụ LSI) bao quát vật liệu, ứng dụng công trình và thông số kỹ thuật.
       - TỰ ĐỘNG BÀN GIAO: Chốt dàn ý H2/H3 chi tiết và chuyển thẳng sang Bước 3 (Biên tập nội dung), không dừng lại ở Bước 2.

    2. CHỐNG ĂN THỊT TỪ KHÓA (CANNIBALIZATION):
       - Tuyệt đối KHÔNG đặt từ khóa chính trùng với từ khóa của bài sản phẩm đã bán trên 2Pro.biz (ví dụ: bài sản phẩm đã giữ từ khóa "giá treo dụng cụ vệ sinh" thì bài blog phải dùng long-tail "cách chọn giá treo dụng cụ vệ sinh").
       - Đảm bảo từ khóa chính có search intent thông tin của người dùng tìm hiểu giải pháp.

    3. MẠNG LƯỚI TOPICAL MAP & LIÊN KẾT NỘI BỘ (INTERNAL LINKS):
       - Quét kho bài viết đã xuất bản trên 2pro.biz, đề xuất 7-10 anchor text liên quan mật thiết.
       - Toàn bộ anchor text bắt buộc phải được in đậm (<a ...><strong>anchor text</strong></a>).
       - Phân bổ anchor text rải rác tự nhiên từ đầu đến cuối bài, không dồn cục vào một khu vực.

    4. THIẾT KẾ DÀN Ý & BÀN GIAO:
       - Đề xuất slug ngắn chuẩn SEO (BẮT BUỘC slug <= 40 ký tự để khi ghép với URL chuyên mục https://2pro.biz/.../ thì tổng URL <= 75 ký tự theo chuẩn Rank Math). Bắt buộc slug phải chứa trọn vẹn từ khóa chính; độ dài từ khóa chính khi nghiên cứu ở Bước 1 phải được tính toán trước để không vượt quá giới hạn này.
       - SEO Title (55-60 ký tự chuẩn XANH Rank Math, áp dụng cẩm nang [[cong-thuc-viet-tieu-de-va-hook-2pro]], chứa từ khóa chính ngay đầu kết hợp số định lượng hoặc lợi ích kỹ thuật để kích thích CTR). BÀI BLOG: TUYỆT ĐỐI KHÔNG thêm 2Pro, Lead hoặc tên thương hiệu vào SEO Title. Thương hiệu chỉ xuất hiện ở H2 cuối bài và khối liên hệ.
       - Meta Description (<920px render width, khoảng 120-135 ký tự, chứa từ khóa chính ở đầu).
       - ĐỊNH HƯỚNG PHẠM VI SẢN PHẨM (SINGLE vs MULTI-PRODUCT INTENT - QUAN TRỌNG):
         + Nếu từ khóa/tiêu đề mang tính tổng quan, cẩm nang lựa chọn danh mục ("Cách chọn...", "Tiêu chuẩn chọn...", "Kinh nghiệm...", "Nên dùng loại nào..."): Dàn ý BẮT BUỘC phải đối chiếu kho sản phẩm thực tế 2Pro (`2pro.biz`), phân bổ thành các phân khúc ứng dụng và giới thiệu đa dạng các dòng/mẫu mã 2Pro đang phân phối (ví dụ: dòng cơ học nút nhấn inox, dòng cần gạt trợ lực, dòng bình đôi đa năng, dòng dung tích lớn). Bảng so sánh phải đối chiếu trực tiếp giữa các dòng sản phẩm của 2Pro. TUYỆT ĐỐI CẤM thiên lệch toàn bộ bài viết vào duy nhất một sản phẩm lẻ.
         + Nếu từ khóa/tiêu đề tập trung vào 1 sản phẩm cụ thể ("Đánh giá hộp xà phòng cần gạt chữ T 450ml..."): Lúc này dàn ý mới đào sâu chuyên biệt vào một sản phẩm đó.
       - Dàn ý H2/H3 ngữ nghĩa sạch sẽ, KHÔNG đánh số thứ tự đầu tiêu đề (trừ khi là danh sách có liên quan đến list).
       - BẮT BUỘC MỖI H2 CHÍNH PHẢI CÓ TỪ 2 ĐẾN 3 THẺ CON H3: Chia nhỏ các góc nhìn kỹ thuật, tính năng, quy trình. Tuyệt đối không để H2 rỗng không có H3 khiến nội dung bị dồn cục thành khối chữ đơn điệu.
       - BẮT BUỘC CÓ H2 CHUYỂN TIẾP TRƯỚC KHỐI LIÊN HỆ: Dàn ý bắt buộc phải có phần H2 tổng kết bài viết và dẫn dắt tự nhiên về thông tin công ty (ví dụ: `<h2>Tổng kết kinh nghiệm và địa chỉ cung ứng [tên sản phẩm] uy tín</h2>`), gồm 2 thẻ con H3: (1) `<h3>Đúc kết các tiêu chí cốt lõi khi lựa chọn cho công trình</h3>` và (2) `<h3>Kho sỉ 2Pro – Đối tác phân phối thiết bị vệ sinh dự án tin cậy</h3>`. Sau đó mới đặt Khối liên hệ, và cuối cùng mới là H2 FAQ.
       - Bàn giao trọn vẹn bộ từ khóa, dàn ý H2/H3 chi tiết và danh sách internal links sang bước Biên tập.

- agent: bien-tap-noi-dung-seo-2pro
  task: |
    Yêu cầu gốc: {{input}}
    Kết quả nghiên cứu dàn ý & từ khóa từ bước 1:
    {{prev}}

    MỤC TIÊU: Viết hoàn chỉnh nội dung bài viết chuyên sâu (CHUẨN 3.000 - 3.700 TỪ) chuẩn AIO/GEO/AEO, tích hợp mạng lưới Topical Map và chuẩn bị gói 4 hình ảnh chuẩn 2Pro.

    1. CHUẨN AIO, GEO & ĐỘ DÀI LÝ TƯỞNG:
       - ĐỘ DÀI BÀI VIẾT: Bắt buộc nằm trong khoảng 3.000 đến 3.700 từ (không vượt quá 3.700 từ).
       - Mở bài Sapo trực diện: Đi thẳng vào giải pháp kỹ thuật và điểm đau vận hành theo cẩm nang [[cong-thuc-viet-tieu-de-va-hook-2pro]], định danh rõ thực thể ngay câu đầu tiên. Cấu trúc 3 câu vàng: Câu 1 nêu giải pháp + từ khóa chính in đậm; Câu 2 nêu rủi ro khi chọn sai; Câu 3 định vị 2Pro là tổng kho vật tư vệ sinh công nghiệp.
       - CẤM TUYỆT ĐỐI câu hỏi tu từ dẫn dắt gián tiếp ("Bạn đang phân vân...", "Bạn có biết...", "Trong thời đại ngày nay...").
       - CẤM cụm từ sáo rỗng ("Tóm lại", "Như đã đề cập ở trên").
       - CẤM TUYỆT ĐỐI dùng: "100%", "tuyệt đối", "chắc chắn" trong nội dung thân bài mô tả tính năng sản phẩm. Thay bằng: "hiệu quả cao", "bảo vệ tối đa", "giảm thiểu rủi ro", "ngăn chặn hiệu quả". (Không áp dụng cho template HTML khối liên hệ cố định).
       - ĐỘ DÀI VÀ CẤU TRÚC ĐOẠN VĂN CHUẨN RANK MATH: Tuyệt đối KHÔNG viết theo kiểu "1 câu 1 dòng" rời rạc, cộc lốc khiến bài viết giống danh sách thiếu tự nhiên. Mỗi đoạn văn <p> phải gồm từ 2 đến 4 câu liên kết mạch lạc, mở rộng và phát triển ý hoàn chỉnh. Độ dài lý tưởng của mỗi đoạn văn <p> là từ 60 đến 90 từ. GIỚI HẠN TỐI ĐA: Tuyệt đối KHÔNG để đoạn văn nào vượt quá 100-110 từ (vì Rank Math coi đoạn trên 120 từ là dài và sẽ báo lỗi đỏ).
       - Không tự bịa số liệu thống kê ảo giác; sử dụng thông số kỹ thuật thực tế của sản phẩm 2Pro.
       - Thuần Việt 100%: Loại bỏ tiếng Anh chêm vào khi đã có thuật ngữ tiếng Việt chuẩn xác.
       - Tiêu đề H2/H3: KHÔNG đánh số thứ tự (1, 1.1, 2...) trừ khi tiêu đề liên quan trực tiếp đến list.
       - CẤU TRÚC PHÂN TẦNG H2/H3 & ĐA DẠNG HÓA HÌNH THỨC TRÌNH BÀY (CHỐNG BỨC TƯỜNG CHỮ - WALL OF TEXT):
         + BẮT BUỘC mỗi H2 chính phải phân nhánh thành 2 đến 3 thẻ con H3 chuyên sâu để bóc tách từng khía cạnh kỹ thuật cụ thể.
         + TUYỆT ĐỐI CẤM tình trạng 1 H2 chỉ gồm 7-8 đoạn văn <p> liên tiếp không có tiêu đề phụ H3 hoặc các yếu tố trực quan ngắt nhịp.
         + ĐA DẠNG HÓA CÁC HÌNH THỨC NỘI DUNG DƯỚI MỖI H2/H3:
           * Đoạn văn tự nhiên mạch lạc (từ 60-90 từ mỗi thẻ <p>, tuyệt đối không vượt quá 110 từ).
           * Danh sách gạch đầu dòng tính năng/ưu thế (<ul><li>).
           * Quy trình hướng dẫn thao tác từng bước có thứ tự (<ol><li>).
           * Hộp checklist kiểm tra thực tế (hộp callout bo góc viền màu với các mục đánh dấu ☑).
           * Bảng số liệu so sánh đối chiếu kỹ thuật (<table>) chuẩn responsive.
           * Khung tóm tắt khuyến nghị lựa chọn theo từng loại hình công trình.
         + NHỊP ĐIỆU THỊ GIÁC (VISUAL RHYTHM): Cứ sau 1-2 đoạn văn ngắn là luân chuyển sang danh sách gạch đầu dòng, checklist, bảng biểu hoặc ảnh minh họa. Giúp độc giả B2B và AI Overviews dễ dàng đọc quét (scan) thông tin trong vài giây.
       - Quy tắc In đậm (De-bolding): CHỈ in đậm từ khóa chính 1 LẦN DUY NHẤT ở câu đầu tiên của Sapo (<strong>...</strong>). Tất cả các lần xuất hiện khác của từ khóa trong thân bài để chữ thường không in đậm.
       - Anchor text liên kết nội bộ: Toàn bộ 7-10 anchor text phải được in đậm (<a ...><strong>anchor text</strong></a>) và rải đều khắp bài.
       - MẬT ĐỘ TỪ KHÓA CHUẨN RANK MATH GREEN ZONE (BẮT BUỘC >= 1.05% - 1.25%): BẮT BUỘC mật độ từ khóa tính trên tổng số từ thực tế phải đạt từ 1.05% đến 1.25% (Rank Math báo lỗi vàng nếu dưới 1.00%). CÔNG THỨC: Số lần xuất hiện = (Tổng số từ bài viết * 1.10%) / 100. Với bài ~3.200 từ: 36-40 lần; bài ~3.700 từ: 41-44 lần; bài dài ~4.000-4.300 từ: BẮT BUỘC xuất hiện 46-50 lần (tuyệt đối không để hụt mức 0.98% / 42 lần khiến Rank Math báo vàng). Rải đều từ khóa vào tiêu đề H2/H3, bullet points và đoạn văn tự nhiên.

    2. QUY TRÌNH HÌNH ẢNH THỰC TẾ & BẢO TOÀN SẢN PHẨM (1 BÌA + 3 THÂN BÀI) - BÁM SÁT [[tieu-chuan-hinh-anh-da-dang-thuc-te-2pro]]:
       - TẤT CẢ 4 ẢNH ĐỀU CÓ: Tỉ lệ chuẩn 8:5 (800x500 px), định dạng WebP, dung lượng nhẹ DƯỚI 60KB (<60KB).
       - PHƯƠNG PHÁP TẠO ẢNH BỐI CẢNH (IMAGE-TO-IMAGE / MULTIMODAL PROMPTING):
         + NGUỒN ẢNH THAM CHIẾU DUY NHẤT (BẮT BUỘC 100% LẤY TỪ KHO SẢN PHẨM 2PRO): Tuyệt đối KHÔNG tìm kiếm hoặc tải ảnh tham chiếu từ Google, Shopee, Lazada hay bất kỳ nguồn bên ngoài nào. Việc lấy ảnh bên ngoài sẽ khiến AI sinh ra sản phẩm sai lệch mẫu mã và màu sắc dị biệt (như màu tím, hồng) mà 2Pro không bán.
         + CƠ CHẾ TRÍCH XUẤT ẢNH GỐC: Agent BẮT BUỘC gọi aafm-get-post theo Product ID đối chiếu trong kế hoạch bài viết (ví dụ Product 24039, 11118, 25228...) để trích xuất trực tiếp URL ảnh sản phẩm thật (featured_image.url từ thư viện WordPress 2Pro) đưa vào tham số images của javis_generate_image (Image-to-Image).
         + Tuyệt đối KHÔNG cắt ghép 2D thủ công từ ảnh nền trắng dán lên background (trông sẽ bị giả, lộ viền, sai đổ bóng và sai góc tụ phối cảnh). AI nhìn thấy sản phẩm thật của 2Pro sẽ tự động tái tạo ánh sáng, vật liệu inox/nhôm, đầu kẹp xanh ngọc/công nghiệp và bóng đổ sàn 3D tự nhiên.
           * CẤM lặp lại cùng 1 tư thế sản phẩm dựng đứng thẳng đơ giữa sàn qua các ảnh.
           * LUÂN PHIÊN CÁC TRẠNG THÁI & GÓC MÁY:
             Mẫu 1 (Thao tác thực tế / Action Shot): "tạo ảnh chụp chân thực, thực tế tại Việt Nam, kích thước 8:5. Nhân viên vệ sinh Việt Nam mặc đồng phục tạp vụ lịch sự gọn gàng, đeo găng tay cao su, đang đẩy [tên sản phẩm] lau sàn trên nền gạch men/sàn epoxy sạch bóng của [nhà máy / bệnh viện / văn phòng]. Góc máy nghiêng tự nhiên, không gian sạch sẽ, chuẩn 5S."
             Mẫu 2 (Trạm dụng cụ / Xe đẩy 5S): "tạo ảnh chụp thực tế góc trạm dụng cụ vệ sinh chuẩn 5S tại Việt Nam, kích thước 8:5. Dụng cụ [tên sản phẩm] được xếp đặt ngay ngắn trên xe đẩy vệ sinh 3 tầng (hoặc treo trên giá kim loại 5S gắn tường theo mã màu). Bối cảnh kho đệm sạch sẽ, ánh sáng rõ ràng, không gian thoáng đãng."
             Mẫu 3 (Ảnh đồ họa minh họa / Infographic): "tạo ảnh đồ họa infographic chuyên nghiệp, kích thước 8:5, phong cách vector hiện đại nền trắng sáng. Minh họa sơ đồ phân vùng mã màu dụng cụ vệ sinh 4 khu vực (hoặc sơ đồ thông số kỹ thuật chi tiết). Chú thích chữ tiếng Việt rõ nét, bố cục cân đối."
       - CHỐNG DỊ TẬT SẢN PHẨM, GIẢI PHẪU CON NGƯỜI & CHỮ RÁC AI (ANTI-MUTATION & ANATOMY GUARDRAILS):
          + DỊ TẬT GIẢI PHẪU CON NGƯỜI (LỖI ĐỎ BẮT BUỘC REJECT):
            * Bàn chân & Giày: Mỗi người CHỈ CÓ ĐÚNG 02 CHÂN và 02 CHIẾC GIÀY. TUYỆT ĐỐI CẤM hiện tượng 3 chân, 3 chiếc giày, hoặc chân mọc thừa từ sau gót gác lên bánh xe đẩy / kệ hàng.
            * Bàn tay: Đủ 5 ngón, không dính ngón, không thừa ngón. Ưu tiên đeo găng tay lao động gọn gàng.
            * Nguyên tắc Đơn hành động: Mỗi người chỉ làm 1 hành động tự nhiên (hoặc đẩy xe, hoặc quỳ kiểm tra khóa bánh, hoặc kéo khay). TUYỆT ĐỐI CẤM giao 2 hành động đối nghịch cùng lúc (vừa cúi thao tác tay bên này vừa với chân ra sau đạp phanh bên kia), vì AI Diffusion sẽ phân rã thành 2 nhánh render sinh ra 3 chân.
            * Ưu tiên Ảnh Tĩnh Sản Phẩm (Still Life) hoặc Cận cảnh thao tác (Close-up hands) khi bối cảnh có nhiều kết cấu kim loại/bánh xe phức tạp.
          + DỊ TẬT DỤNG CỤ: TUYỆT ĐỐI CẤM sản phẩm biến dạng / lộ AI rõ rệt: Cây gạt nước "2 đầu" (trên đỉnh chuôi cầm lại mọc thêm lưỡi gạt cao su trong khi đáy dưới đã có bàn gạt sàn); chổi mọc thêm đầu lau; cán xuyên qua nhau; khớp nối méo mó.
          + CHỮ RÁC AI: TUYỆT ĐỐI CẤM chữ rác AI (ký tự vô nghĩa, chữ tượng hình, chữ tiếng Nga/Cyrillic như "СПЕЦМОПОВ") trên biển hiệu, nhãn tường hay thùng đồ. Biển hiệu chỉ dùng tiếng Việt chuẩn hoặc để bảng trơn phẳng không chữ.
          + Khi sinh ảnh trạm dụng cụ: Ưu tiên bố cục thoáng trên xe đẩy dọn vệ sinh 3 tầng (Janitor trolley) chuẩn để AI phân tách từng món độc lập.
        - ĐỒNG BỘ 100% GIỮA ẢNH VÀ CAPTION (CAPTION-VISUAL CONSISTENCY):
         + QUY TẮC CỐT LÕI: Caption bên dưới ảnh CHỈ ĐƯỢC miêu tả đúng các dụng cụ thực tế có trong ảnh.
         + TUYỆT ĐỐI CẤM trường hợp "ảnh một đằng, caption một nẻo" (ví dụ: Caption ghi có chổi, cây gạt nước, hót rác nhưng ảnh chỉ có cây lau và xô). Nếu ảnh thiếu món nào, caption bắt buộc phải viết lại cho khớp đúng với ảnh.
         + Trước khi gán caption, agent BẮT BUỘC dùng `javis_describe_image` để kiểm tra các vật thể có thật trong ảnh.
       - DANH MỤC BỘ 4 ẢNH CỦA BÀI VIẾT:
         + 01 Ảnh bìa (Cover Banner): BẮT BUỘC tạo mới theo chuẩn tỉ lệ 8:5 (800x500 px), bố cục split-screen (Trái 42%: flat graphic panel ít chữ, nổi bật, căn lề an toàn >=45px; Phải 58%: ảnh sản phẩm thật trong bối cảnh thực tế). MÀU SẮC BẮT BUỘC trích xuất từ ảnh sản phẩm thực tế - KHÔNG dùng màu navy/slate tối cố định cho mọi bài (inox → xám than+vàng cam; nhựa ABS → xanh slate+trắng sứ; cao su/bảo hộ → vàng amber+cam; gỗ/thảm → nâu đất+vàng cát). CHỮ trên ảnh tối giản: 01 tiêu đề chính in hoa + 01 dòng phụ ngắn, không nhồi nhét text. BẮT BUỘC tuân thủ skill [[blog-cover-image]] và cẩm nang [[cong-thuc-tao-anh-bia-blog-gemini-style]], sử dụng kết nối tạo ảnh (Gemini hoặc ChatGPT) đã cấu hình trên hệ thống Javis để sinh ảnh bìa chuẩn tỉ lệ 8:5 (800x500 px): khung kính mờ bên trái chứa typography tiếng Việt chuẩn xác, bối cảnh người/sản phẩm bên phải chuẩn tỷ lệ 1:1, tuyệt đối không bóp méo hay co kéo sản phẩm.
         + 01 Ảnh sơ đồ kỹ thuật gốc hoặc ảnh đồ họa minh họa Infographic: Bảo toàn thông số, kích thước hoặc sơ đồ phân vùng mã màu rõ nét.
         + 02 Ảnh bối cảnh thực tế đa dạng: 01 ảnh nhân viên đang thao tác thực tế (Action Shot) và 01 ảnh bố trí trạm dụng cụ / xe đẩy chuẩn 5S (Storage Shot). Tuyệt đối không để 2 ảnh cùng đứng thẳng đơ một tư thế.
       - NGUYÊN TẮC CHỌN ẢNH THÂN BÀI & BỘ LỌC THỊ GIÁC (VISION VALIDATION):
         + CƠ CHẾ XEM ẢNH THẬT BẰNG VISION (javis_describe_image): Khi chọn ảnh từ Media Library hoặc sau khi sinh ảnh mới, Javis KHÔNG ĐƯỢC chỉ nhìn vào tên file hay alt text. BẮT BUỘC dùng công cụ javis_describe_image để kiểm tra trực quan sản phẩm trong ảnh:
           * Chất liệu thực tế: Nếu mục viết về nhựa ABS thì ảnh PHẢI là vỏ nhựa ABS; nếu mục viết về inox 304 thì ảnh PHẢI là kim loại inox. Tuyệt đối không cắm râu ông nọ cắm cằm bà kia.
           * Kiểm định giải phẫu người (Human Anatomy Check): Nếu ảnh có người, kiểm tra kỹ đếm đủ 2 chân, 2 tay, không có chân/giày thứ 3 mọc thừa từ sau gót hay bánh xe. Nếu phát hiện dị tật giải phẫu, BẮT BUỘC REJECT và sinh lại ảnh.
           * Nhận diện thương hiệu: Kiểm tra xem ảnh có gắn logo, nhãn mác hoặc bối cảnh của bên khác (như Sóng Vàng hay các shop sàn TMĐT) hay không. TUYỆT ĐỐI CẤM nhắc hoặc dùng ảnh của Sóng Vàng / đơn vị khác trong bài blog 2Pro.
           * Kiểm tra chữ đồ họa: Đảm bảo ảnh KHÔNG có text đồ họa to (không phải ảnh bìa của bài viết khác).
         + NGUYÊN TẮC THƯƠNG HIỆU ĐỘC QUYỀN 2PRO: Bài viết thuộc blog 2pro.biz, nghiêm cấm quảng bá hoặc gắn tên thương hiệu bên ngoài như Sóng Vàng. Định vị duy nhất là Tổng kho vật tư vệ sinh 2Pro (CÔNG TY TNHH ĐẦU TƯ LEAD).
       - PHÂN BỔ VỊ TRÍ ĐẶT ẢNH CHUẨN UX (CHỐNG DỒN CỤC ẢNH):
         + Chia đều theo nhịp thị giác ~1.000 từ / 1 ảnh:
           * Ảnh 1: Đặt ở Phần 1 (sau phần phân tích nguyên lý chống ẩm mốc & kiểm soát nhiễm khuẩn).
           * Ảnh 2: Đặt ở Phần 2 (sau phần phân tích cơ chế ngàm kẹp con lăn cao su).
           * Ảnh 3: Đặt ở Phần 3 (ngay trước Bảng đối chiếu so sánh thông số kỹ thuật).
       - Cách chèn ảnh thân bài trong HTML: BẮT BUỘC dùng shortcode caption chuẩn của WordPress:
         [caption id="attachment_ID" align="aligncenter" width="800"]<img style="max-width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.08);" src="URL" alt="ALT" width="800" height="500" /> Chú thích kỹ thuật thực tế cho người đọc[/caption]

    3. CẤU TRÚC H2 CHUYỂN TIẾP TỰ NHIÊN & KHỐI LIÊN HỆ CHUẨN (CHỐNG ĐỘT NGỘT):
       - TUYỆT ĐỐI CẤM thả khối liên hệ đột ngột ngay sau mục hướng dẫn kỹ thuật hoặc bảo dưỡng.
       - BẮT BUỘC PHẢI CÓ 1 PHẦN H2 RIÊNG LÀM CẦU NỐI: `<h2>Tổng kết kinh nghiệm và địa chỉ cung ứng [tên sản phẩm] uy tín</h2>` (hoặc tiêu đề tương đương theo chủ đề bài viết).
       - NỘI DUNG CỦA H2 CHUYỂN TIẾP NÀY GỒM:
         + 01 đoạn dẫn tóm tắt giá trị vận hành và giải pháp cho công trình.
         + Thẻ con `<h3>Đúc kết các tiêu chí cốt lõi khi lựa chọn cho công trình</h3>`: Chứa danh sách bullet points (<ul><li>) tóm tắt nhanh 4-5 tiêu chuẩn then chốt đã phân tích trong bài.
         + Thẻ con `<h3>Kho sỉ 2Pro – Đối tác phân phối thiết bị vệ sinh dự án tin cậy</h3>`: Đoạn văn chuyển tiếp tự nhiên giới thiệu vị thế Tổng kho vật tư vệ sinh 2Pro (CÔNG TY TNHH ĐẦU TƯ LEAD) – nhà phân phối trực tiếp số lượng lớn cho các dự án khách sạn, tòa nhà, bệnh viện trên toàn quốc với giá sỉ tận gốc, đầy đủ linh kiện thay thế và hóa đơn VAT.
       - NGAY DƯỚI PHẦN DẪN DẮT TRÊN MỚI LÀ KHỐI LIÊN HỆ CHUẨN (BẮT BUỘC COPY NGUYÊN VĂN 100% ĐOẠN HTML DƯỚI ĐÂY, CẤM TỰ Ý RÚT GỌN LÀM MẤT 2 NÚT BẤM GỌI/ZALO VÀ BADGE):
         ```html
         <div style="background: #ffffff; border: 2px solid #22c55e; border-radius: 12px; padding: 24px; margin: 32px 0; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; box-shadow: 0 4px 12px rgba(34, 197, 94, 0.08);">
           <!-- Header Card -->
           <div style="display: flex; justify-content: space-between; align-items: center; border-bottom: 1px solid #dcfce7; padding-bottom: 12px; margin-bottom: 14px;">
             <span style="font-size: 16px; font-weight: 800; color: #15803d; text-transform: uppercase;">CÔNG TY TNHH ĐẦU TƯ LEAD</span>
             <span style="background: #dcfce7; color: #166534; font-size: 12px; font-weight: 700; padding: 4px 12px; border-radius: 20px;">Kho sỉ 2Pro</span>
           </div>
         
           <!-- Thông tin pháp nhân -->
           <p style="margin: 0 0 8px 0; font-size: 14.5px; color: #4b5563;"><strong>Văn phòng điều hành:</strong> Số 10/2 Phan Trọng Tuệ, xã Đại Thanh, TP. Hà Nội</p>
           <p style="margin: 0 0 16px 0; font-size: 14.5px; color: #4b5563;">
             <strong>Kênh thông tin:</strong> <a href="https://2pro.biz/" target="_blank" rel="noopener" style="color: #16a34a; font-weight: 600; text-decoration: none;">2pro.biz</a> 
             <span style="color: #cbd5e1; margin: 0 6px;">-</span> 
             <strong>Fanpage:</strong> <a href="https://www.facebook.com/thietbivadungcuvesinh2pro/" target="_blank" rel="noopener" style="color: #16a34a; font-weight: 600; text-decoration: none;">2Pro</a>
           </p>
         
           <!-- Khung nổi bật Số điện thoại & 2 Nút bấm dài -->
           <div style="background-color: #f0fdf4; border-radius: 10px; padding: 16px 20px; display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: 16px;">
             <div>
               <span style="display: block; font-size: 12px; color: #6b7280; font-weight: 700; text-transform: uppercase; letter-spacing: 0.3px;">Tư vấn kỹ thuật & Chiết khấu dự án:</span>
               <span style="font-size: 22px; font-weight: 800; color: #15803d; line-height: 1.3;">0974.947.391</span>
             </div>
             
             <div style="display: flex; flex-wrap: wrap; gap: 12px;">
               <!-- Nút Gọi Trực Tiếp (Kéo dài) -->
               <a href="tel:0974947391" style="display: inline-flex; align-items: center; justify-content: center; min-width: 140px; background-color: #15803d; color: #ffffff; padding: 12px 24px; border-radius: 8px; text-decoration: none; font-weight: 700; font-size: 15px; box-shadow: 0 2px 4px rgba(21, 128, 61, 0.2);">
                 📞 Gọi trực tiếp
               </a>
               <!-- Nút Nhắn Zalo (Kéo dài) -->
               <a href="https://zalo.me/0974947391" target="_blank" rel="noopener" style="display: inline-flex; align-items: center; justify-content: center; min-width: 140px; background-color: #0068ff; color: #ffffff; padding: 12px 24px; border-radius: 8px; text-decoration: none; font-weight: 700; font-size: 15px; box-shadow: 0 2px 4px rgba(0, 104, 255, 0.2);">
                 💬 Nhắn Zalo
               </a>
             </div>
           </div>
         </div>
         ```
       - Cấu trúc FAQ ở cuối bài: 3-4 câu hỏi thực tế của khách hàng. Câu đầu tiên của mỗi phần trả lời bắt buộc đi thẳng vào đáp án với độ dài 40-60 từ.

    4. BÀN GIAO:
       - Nội dung HTML hoàn chỉnh (không chứa thẻ <h1>).
       - Bàn giao trọn vẹn: Tiêu đề H1, SEO Title, Meta Description, Slug, Danh mục ("Review sản phẩm" ID 17), Chuỗi Focus Keyword, Ảnh bìa ID/URL.

- agent: xuat-ban-wordpress-2pro
  task: |
    Yêu cầu gốc: {{input}}
    Nội dung hoàn chỉnh từ bước biên tập:
    {{prev}}

    MỤC TIÊU: Đăng hoặc cập nhật bản nháp (DRAFT) lên WordPress 2Pro và cấu hình Rank Math SEO tối ưu.

    1. NGUYÊN TẮC AN TOÀN:
       - LUÔN để trạng thái bài viết là DRAFT (bản nháp). Không publish, không schedule.
       - Danh mục: ID 17 ("Review sản phẩm").
       - Không tạo thêm post trùng lặp; nếu có post_id mục tiêu thì cập nhật đúng post đó.

    2. CẬP NHẬT NỘI DUNG & HÌNH ẢNH (BỘ LỌC NGHIỆM THU BẮT BUỘC TRƯỚC KHI LƯU - GUARDRAILS):
       - KIỂM TRA H2 CHUYỂN TIẾP & KHỐI LIÊN HỆ: Kiểm tra xem trước Khối liên hệ đã có thẻ H2 tổng kết bài viết và dẫn dắt về năng lực công ty 2Pro hay chưa. Tuyệt đối không để khối liên hệ xuất hiện đột ngột dưới mục kỹ thuật/bảo dưỡng. Kiểm tra Content HTML có đủ cả 2 nút bấm `href="tel:0974947391"` và `href="https://zalo.me/0974947391"` cùng badge `Kho sỉ 2Pro`. Nếu phát hiện bài viết bị thiếu H2 chuyển tiếp hoặc khối liên hệ bị rút gọn, agent bước này BẮT BUỘC tự động bổ sung H2 chuyển tiếp và chèn đúng đoạn HTML chuẩn đầy đủ vào trước thẻ `<h2>Câu hỏi thường gặp`.
       - KIỂM TRA PHÂN TẦNG H2/H3: Đảm bảo mọi H2 đều có từ 2-3 H3 chuyên biệt, không có hiện tượng dồn cục đoạn văn <p>.
       - KIỂM TRA ĐỊNH DẠNG TRỰC QUAN: Đảm bảo bài viết có danh sách bullet (<ul>), quy trình từng bước (<ol>), bảng so sánh (<table>).
       - KIỂM TRA DE-BOLDING & TỪ KHÓA: Từ khóa chính chỉ in đậm 1 lần duy nhất ở Sapo; mật độ từ khóa BẮT BUỘC đạt chuẩn >= 1.05% - 1.25% tính theo tổng số từ thực tế: `Số lần = Tổng số từ * 1.1% / 100` (Bài ~3.500 từ cần 40-44 lần, bài ~4.200 từ cần 46-50 lần). Tuyệt đối không để hụt dưới 1.00% (như mức 0.98% / 42 lần). Nếu phát hiện thiếu, agent bước này phải chủ động bổ sung tự nhiên vào các đoạn văn trước khi lưu.
       - KIỂM TRA ANCHOR TEXT: Toàn bộ 7-10 anchor text liên kết nội bộ phải được in đậm (<a ...><strong>...</strong></a>).
       - BẮT BUỘC TRUYỀN THAM SỐ `slug` TRONG CẢ `aafm-create-draft` LẪN `aafm-update-post`: Slug BẮT BUỘC phải là dạng không dấu của từ khóa chính (≤40 ký tự), các từ cách nhau bằng dấu gạch ngang `-` (ví dụ từ khóa chính "bộ dụng cụ lau kính tòa nhà gồm những gì" -> slug `bo-dung-cu-lau-kinh-toa-nha-gom-nhung-gi`). TUYỆT ĐỐI KHÔNG được giữ slug cũ lệch với từ khóa chính mới khi sửa bài cũ, vì Rank Math sẽ báo lỗi đỏ "Không tìm thấy từ khoá chính trong URL này"!
       - Ghi nhận Title, Slug, Content HTML đã chuẩn hóa, Featured Media vào WordPress post.
       - KIỂM TRA ĐOẠN VĂN VÀ CẤU TRÚC: Tuyệt đối không để tình trạng "1 câu 1 dòng". Đảm bảo mỗi thẻ <p> là đoạn văn 2-4 câu (60-90 từ). Kiểm tra không để đoạn văn nào vượt quá 100-110 từ (tránh lỗi đỏ Rank Math >120 từ).
       - KIỂM TRA TỪ CẤM ĐẢM BẢO: Không để lọt các từ "100%", "tuyệt đối", "chắc chắn" trong thân bài.
       - KIỂM TRA KHỐI LIÊN HỆ: Tuyệt đối cấm layout 3 cột và số điện thoại lạ (0965, 0818). Bắt buộc chỉ dùng số 0974.947.391, 2 nút Gọi + Zalo và badge Kho sỉ 2Pro.

    3. CẤU HÌNH RANK MATH SEO:
       - Sử dụng công cụ `wordpress-2pro-bai-nhap__aafm-rankmath-update-post` để cập nhật:
         + focus_keyword: Chuỗi từ khóa phân cách dấu phẩy, từ khóa chính đứng đầu tiên.
         + title: SEO Title (55-60 ký tự chuẩn XANH Rank Math, ĐỐI VỚI BÀI BLOG: TUYỆT ĐỐI KHÔNG chứa "2Pro" hoặc "Lead" trong SEO Title).
         + description: Meta description (<920px render width, ~120-135 ký tự, không chứa "2Pro").
         + og_title: Giống SEO Title (không chứa 2Pro).
         + og_description: Giống Meta description.
         + og_image & twitter_image: URL ảnh bìa đính kèm từ Media Library.
         + canonical: BẮT BUỘC đặt canonical chuẩn `https://2pro.biz/review-san-pham/{slug}/`.
         + robots: BẮT BUỘC luôn đặt "index", TUYỆT ĐỐI CẤM truyền "noindex" hay "noindex,nofollow".

    4. BÁO CÁO KẾT QUẢ:
       - Trả về Post ID, Preview URL (https://2pro.biz/?p=ID), điểm Rank Math và tóm tắt nghiệm thu để chuyển sang Bước 5 ghi nhận tiến độ.

- agent: bao-cao-audit-sheet-2pro
  task: |
    Yêu cầu gốc: {{input}}

    Kết quả đăng nháp WordPress từ bước trước:
    {{prev}}

    MỤC TIÊU: Tự động ghi nhận thông tin bài blog mới vừa tạo vào Google Sheet theo dõi tiến độ công việc của 2Pro.

    1. THÔNG TIN BẢNG TÍNH GOOGLE SHEET:
       - Spreadsheet ID: 1UZ2fuxKH5tXYXrtzDspHbKY7rFcZemBLvYvoBFcU4ko
       - Dải ô: Đọc `A1:A5000` qua `google-workspace__read_sheet_values` để xác định dòng trống tiếp theo: `next_row = dòng_cuối + 1`.

    2. CẤU TRÚC ĐIỀN ĐỦ 11 CỘT (A:K) TẠI DÒNG `next_row`:
       - Cột A (Ngày): Ngày thực hiện (định dạng DD/MM, ví dụ: 20/11).
       - Cột B (Công việc): `Blog`.
       - Cột C (Tiêu đề post/ sản phẩm): Tiêu đề hiển thị của bài viết.
       - Cột D (Từ khóa chính): Focus Keyword của bài viết.
       - Cột E (Từ khóa phụ): Danh sách các từ khóa phụ (phân cách bằng dấu phẩy).
       - Cột F (Thương hiệu): `2Pro`.
       - Cột G (Người thực hiện): `Ly`.
       - Cột H (Link content): URL permalink chuẩn của bài viết trên web (`https://2pro.biz/review-san-pham/{slug}/`). TUYỆT ĐỐI KHÔNG dùng link thô `https://2pro.biz/?p=ID`.
       - Cột I (Trạng thái): `Đã hoàn thành`.
       - Cột J (Index): `Chưa index` (đối với bản nháp mới tạo).
       - Cột K (Tình trạng): `Chưa yêu cầu Google index lại`.

    3. GHI VÀ BÁO CÁO:
       - Gọi `google-workspace__modify_sheet_values` với dải ô `A{next_row}:K{next_row}` và `value_input_option: "USER_ENTERED"`.
       - Đồng thời, cập nhật trạng thái đề tài tương ứng trong file `D:\Javis OS\brains\2Pro SEO\work\content-pipeline-2pro.md` (hoặc GitHub `plans/content-pipeline-2pro.md`) từ `Pending` sang `Done (Post {post_id})`.
       - Báo cáo hoàn tất dòng vừa thêm và đính kèm link Google Sheet: https://docs.google.com/spreadsheets/d/1UZ2fuxKH5tXYXrtzDspHbKY7rFcZemBLvYvoBFcU4ko/edit

updated: '2026-11-20'
---

Nghiên cứu cơ hội từ Content Pipeline/GSC, biên tập nội dung people-first chuẩn AIO/GEO kèm bộ ảnh thực tế và đăng nháp WordPress 2Pro với Rank Math hoàn chỉnh, sau đó tự động ghi nhận báo cáo tiến độ vào Google Sheet theo dõi qua 5 bước tinh gọn.
