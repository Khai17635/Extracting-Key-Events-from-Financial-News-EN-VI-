📌 Các Tính Năng Cốt Lõi
Hệ thống giải quyết đồng thời 3 bài toán NLP quan trọng trên cùng một kiến trúc mô hình[cite: 1]:

Nhận diện thực thể (NER):

Trích xuất Tổ chức (ORG), Số tiền (MONEY), Hành động (ACT) và Tỷ lệ (PERC)[cite: 1].

Sử dụng định dạng gán nhãn BIO chuẩn[cite: 1].

Phân loại sự kiện (Event Classification):

Tự động phân loại văn bản vào 6 nhóm sự kiện trọng tâm: IPO, Hack/Tấn công mạng, M&A (Sáp nhập), Biến động giá, Thay đổi nhân sự, và Kết quả tài chính[cite: 1].

Hỗ trợ hoàn toàn song ngữ Anh - Việt[cite: 1].

Phân tích cảm xúc (Sentiment Analysis):

Xác định thái độ thị trường: Tích cực (Positive), Tiêu cực (Negative), và Trung lập (Neutral)[cite: 1].

Đạt chỉ số F1-score xấp xỉ 0.82[cite: 1].

🧠 Kiến Trúc Mô Hình
Dự án sử dụng mô hình ngôn ngữ lớn làm "xương sống" (Backbone) để xử lý đa nhiệm:

Model: XLM-RoBERTa (base)[cite: 1].

Dữ liệu huấn luyện: Kết hợp tập dữ liệu quốc tế FinancialPhraseBank và dữ liệu thực tế cào từ CafeF, Reuters, Bloomberg[cite: 1].

Pipeline: SentencePiece Tokenizer -> XLM-RoBERTa Encoder -> 3 Classification Heads (NER, Event, Sentiment)[cite: 1].

🛠 Công Nghệ Sử Dụng
Ngôn ngữ: Python[cite: 1].

Thư viện Deep Learning: PyTorch, HuggingFace Transformers[cite: 1].

Web Scraping: BeautifulSoup4, Requests[cite: 1].

Deployment: Flask (Backend), ngrok (Tunneling), Google Colab[cite: 1].

🚀 Hướng Dẫn Chạy Demo
Do mô hình có kích thước lớn (~1.1GB), dự án được tối ưu để chạy trên môi trường Google Colab.

Mở file notebook: NLP_project.ipynb trên Google Colab[cite: 1].

Cài đặt thư viện: Chạy ô cell đầu tiên để cài đặt các dependency cần thiết[cite: 1].

Load Weights: Đảm bảo bạn đã tải các thư mục model (sentiment_model_final, ner_model_final, event_model_final) vào Google Drive cá nhân[cite: 1].

Khởi động Flask App: Chạy ô cell chứa script Flask và ngrok để nhận link truy cập công khai[cite: 1].
