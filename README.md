# Fashion MNIST Clothes Classification

Một project nhỏ để **phân loại quần áo** sử dụng bộ dữ liệu **Fashion-MNIST** bằng Keras/TensorFlow.

Dataset này gồm ảnh grayscale kích thước **28×28**, thuộc **10 lớp** quần áo như T-shirt, Trouser, Sneaker, … :contentReference[oaicite:0]{index=0}

## Nội dung repo
- `FashionMNIST.ipynb` — Notebook chính để load dữ liệu, xây dựng mô hình, huấn luyện và đánh giá.
- `README.md` — Tệp mô tả project này.

## Mô tả bài toán
Bài toán là **phân loại ảnh quần áo** đầu vào thành 1 trong 10 nhãn:
0: T-shirt/top
1: Trouser
2: Pullover
3: Dress
4: Coat
5: Sandal
6: Shirt
7: Sneaker
8: Bag
9: Ankle boot

🛠️ Cách xây dựng mô hình

Trong notebook bạn sử dụng mô hình MLP đơn giản với các tầng:

- Flatten input (28,28,1) → vector 784
- Dense 512 + ReLU
- Dense 256 + ReLU
- Dense softmax 10 lớp

Mô hình được compile với Adam và loss Sparse Categorical Crossentropy.

🚀 Cách chạy

1. Clone repo:
git clone https://github.com/minhchau-creator/fashion_MNIST.git
cd fashion_MNIST

2. Mở notebook:
jupyter notebook FashionMNIST.ipynb

Chạy các cell để:
- load và tiền xử lý dataset
- xây dựng và huấn luyện mô hình
- đánh giá accuracy

📊 Kết quả

Notebook sẽ hiển thị:
- Training / validation accuracy
- Loss curve
  
💻 Công nghệ sử dụng
- Python
- TensorFlow / Keras
- Jupyter Notebook
