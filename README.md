Vector_AutoPlay/
│
├── data/
│   ├── raw/                   # Dữ liệu video gốc chưa qua xử lý
│   ├── processed/             # Dữ liệu sau khi qua tiền xử lý (ảnh hoặc video frame)
│   ├── labeled/               # Dữ liệu sau khi gán nhãn
│   ├── train/                 # Dữ liệu dùng cho training
│   └── test/                  # Dữ liệu dùng cho testing
│
├── models/
│   ├── lstm_model.py          # Mô hình LSTM chính dùng cho dự đoán hành động
│   ├── cnn_feature_extractor.py # CNN dùng để trích xuất đặc trưng từ video frame
│   └── trained_model/         # Thư mục lưu mô hình đã được huấn luyện
│
├── utils/
│   ├── data_preprocessing.py  # Các hàm tiền xử lý dữ liệu
│   ├── video_to_frames.py     # Chuyển đổi video thành từng frame để phân tích
│   ├── annotation_tool.py     # Công cụ hỗ trợ gán nhãn cho dữ liệu video
│   └── helper_functions.py    # Các hàm hỗ trợ khác
│
├── scripts/
│   ├── train_model.py         # Script để huấn luyện mô hình LSTM
│   ├── evaluate_model.py      # Script để đánh giá độ chính xác của mô hình
│   └── run_inference.py       # Script để chạy mô hình và dự đoán hành động trong game
│
├── notebooks/
│   ├── EDA.ipynb              # Notebook phân tích dữ liệu ban đầu (Exploratory Data Analysis)
│   ├── Model_Training.ipynb   # Notebook huấn luyện mô hình và thử nghiệm
│   └── Model_Evaluation.ipynb # Notebook đánh giá mô hình
│
├── config/
│   └── config.yaml            # File cấu hình cho dự án (đường dẫn dữ liệu, tham số huấn luyện, etc.)
│
├── results/
│   ├── logs/                  # Lưu trữ log quá trình huấn luyện và chạy mô hình
│   ├── metrics/               # Lưu trữ các file kết quả đánh giá (accuracy, loss, etc.)
│   └── predictions/           # Lưu trữ kết quả dự đoán từ mô hình
│
├── README.md                  # Mô tả tổng quan về dự án, cách cài đặt và hướng dẫn sử dụng
├── requirements.txt           # Danh sách thư viện cần thiết để chạy dự án
└── main.py                    # File chính để khởi chạy dự án
