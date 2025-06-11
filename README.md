# face-mask-detection-using-cnn
Face Mask Detection using CNN is a deep learning project that detects whether a person is wearing a face mask or not using a Convolutional Neural Network (CNN).

---

## 📌 Project Highlights

- 🔍 Binary classification: With Mask / Without Mask
- 🧠 Deep Learning (CNN) based model
- 📊 High accuracy with simple architecture

---

## 🧱 Model Architecture

- 2D Convolutional Layers
- MaxPooling
- Dropout for regularization
- Flatten + Dense Layers
- Softmax output (2 classes)



###   model summary
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┓
┃ Layer (type)                    ┃ Output Shape           ┃       Param # ┃
┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━┩
│ conv2d (Conv2D)                 │ (None, 125, 125, 32)   │         1,568 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ max_pooling2d (MaxPooling2D)    │ (None, 62, 62, 32)     │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ conv2d_1 (Conv2D)               │ (None, 59, 59, 16)     │         8,208 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ max_pooling2d_1 (MaxPooling2D)  │ (None, 29, 29, 16)     │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ flatten (Flatten)               │ (None, 13456)          │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dense (Dense)                   │ (None, 64)             │       861,248 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dropout (Dropout)               │ (None, 64)             │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dense_1 (Dense)                 │ (None, 32)             │         2,080 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dropout_1 (Dropout)             │ (None, 32)             │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dense_2 (Dense)                 │ (None, 2)              │            66 │
└─────────────────────────────────┴────────────────────────┴───────────────┘
 Total params: 2,619,512 (9.99 MB)
 Trainable params: 873,170 (3.33 MB)
 Non-trainable params: 0 (0.00 B)
 Optimizer params: 1,746,342 (6.66 MB)


 ###  Results

 - Accuracy: **~96%**
- Loss: **< 0.3**
 
