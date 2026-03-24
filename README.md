# TEP – Tài liệu Giáo dục NLP và Transformer

Repository này chứa các notebook Jupyter giáo dục về **Transformer**, **NLP** (Xử lý Ngôn ngữ Tự nhiên) và các phép toán tensor. Tất cả nội dung được viết bằng **tiếng Việt** và có thể mở trực tiếp trong **Google Colab**.

---

## 📒 Danh sách Notebooks

### 1. Xây dựng cơ chế tự chú ý và kiến trúc máy biến áp (GPT-2) từ đầu

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tranthithuvan555-wq/TEP/blob/main/Self_Attention_Transformer_GPT2.ipynb)

**File:** `Self_Attention_Transformer_GPT2.ipynb`

Notebook này hướng dẫn xây dựng từng thành phần của kiến trúc Transformer và GPT-2 từ đầu bằng PyTorch:
- Cơ chế **Self-Attention** (tự chú ý): Query, Key, Value và công thức Attention
- **Multi-Head Attention**: chạy nhiều attention head song song
- **Positional Encoding**: mã hóa vị trí bằng hàm sin/cos
- **Feed-Forward Network** và **Layer Normalization**
- Xây dựng **GPT-2** đơn giản và demo sinh văn bản (text generation)

---

### 2. Máy biến áp được đào tạo trước (BERT, GPT) và đào tạo trên ngôn ngữ đơn giản hóa

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tranthithuvan555-wq/TEP/blob/main/Pretrained_Transformers_BERT_GPT.ipynb)

**File:** `Pretrained_Transformers_BERT_GPT.ipynb`

Notebook này hướng dẫn sử dụng các mô hình pre-trained và fine-tuning:
- **Transfer Learning** trong NLP và tại sao pre-training quan trọng
- **BERT** (PhoBERT cho tiếng Việt): kiến trúc, MLM, NSP và demo fill-mask
- **GPT-2**: kiến trúc autoregressive và demo text generation
- **Fine-tuning** GPT-2 trên tập dữ liệu tiếng Việt và đánh giá kết quả (perplexity)

---

### 3. Ghi chú về quy tắc tổng Einstein (Einstein Summation Convention)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tranthithuvan555-wq/TEP/blob/main/Einstein_Summation_Notes.ipynb)

**File:** `Einstein_Summation_Notes.ipynb`

Notebook này trình bày quy tắc tổng Einstein và cách dùng `einsum` trong NumPy/PyTorch:
- Lịch sử và ý nghĩa của quy tắc tổng Einstein
- Các phép toán cơ bản: dot product, nhân ma trận, chuyển vị, trace, outer product
- Ứng dụng trong Deep Learning: tính attention scores, batch matrix multiplication, tensor contraction
- So sánh `einsum` với các phép toán thông thường về hiệu suất và tính dễ đọc

---

## 🛠️ Yêu cầu

- Python 3.8+
- PyTorch
- NumPy
- HuggingFace Transformers (cho Notebook 2)
- Matplotlib

Tất cả dependencies đều được cài đặt tự động trong cell đầu tiên của mỗi notebook khi chạy trên Google Colab.

## 📌 Cách sử dụng

1. Nhấn nút **"Open in Colab"** trên notebook bạn muốn mở
2. Chọn **Runtime → Run all** để chạy toàn bộ notebook
3. Hoặc chạy từng cell một để học từng bước