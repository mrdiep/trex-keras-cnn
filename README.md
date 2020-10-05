# Huấn luyện game T-Rex sử dụng Keras CNN

## T-rex game
[http://www.trex-game.skipser.com](http://www.trex-game.skipser.com)


### Install Requirement
```
pip install -r requirements.txt
```

## Hướng dẫn

### Bước 1. Thu thập dữ liệu để trainning
- Dữ liệu là screenshot và action hiện tại: nhấn phím lên ↑ , xuống ↓, chạy →

- chạy tool [collect_data.py]: Bạn chơi game, tool sẽ tự record lại và xuất ra folder img làm dữ liệu mẫu.

| Key              | Description                 |
| ---------------- | --------------------------- |
| Up Arrow (↑)     | T-Rex nhẩy                  |
| Down Arrow (↓)   | T-Rex ngồi                |
| Right Arrow (→)  | T-Rex chạy            |


### Bước 2. Training

Chạy file [train.py]
app sẽ đọc dữ liệu bước 1 làm data để train, output là file trex_weight.h5
Training sẽ dùng mạng CNN (mạng tích chập): nó tự tìm ra filter để ra output cho ra 3 label action tương ứng.

### Bước 3. Test laị kết quả: AI chơi game

chạy file [player.py]

```bash
python player.py
```

## Contributing
Feel free to contribute on this project, I will be happy to work with you.

## License
The MIT License (MIT)
