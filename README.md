# Human Activity Recognition (HAR)

This framework focuses on **Human Activity Recognition (HAR)** problems by using machine learning techniques, fine-tuning based on pretrain model such as ResNet50 and Bi-LSTM in combination. The goal is to create a model that can classify human activities when user feed model videos (in any terms of camera angles, resolution, quality).
<--video demo shortly-->

*Note: CSC16004 – Computer Vision - Final Project Rework - 22TGMT HCMUS* 

## News
- 3-12-2025: Add Hugging Face Space for Web Inference demo.
## Installation
### 📥 Clone the Repository
```bash
git clone https://github.com/BAoD1nH/BD_HAR_25.git --recursive
cd BD_HAR_25
```

### ⚙️ Environment Setup
```bash
pip install -r Source/requirements.txt
```

### ⭐ Data preparation
```bash
python Source/dataset_download.py
```

### 🎨 Training model
```bash
python Source/main.py <type-of-dataset> <dataset-path>
```
E.g.
```bash
python Source/main.py ucf11 dataset/ucf11_updated_mpg
```
### 🎯 Inference
```bash
python Source/Inference.py <type-of-dataset> <test_video-path> <model-path>
```

E.g.
```bash
python Source/inference.py ucf11 test_videos/basketball.mp4 Source/models/ucf11_lstm_model.pt
```

## Contributors
- **[Hoàng Bảo Khanh]** - [github/hbkhanh22], FIT HCMUS-VNU
- **[Đinh Nguyễn Gia Bảo]** - [github/BAoD1nH], FIT HCMUS-VNU

## License
- This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
- Any questions please contact via baodinhtfb@gmail.com

> If you find this project useful, please give it a star ⭐️! Contributions are also welcome.
