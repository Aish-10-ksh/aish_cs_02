# 🖼️ Image Encryption Tool (Python)

This project is a **simple image encryption and decryption tool** written in Python. It manipulates pixel values using a basic formula to encrypt or decrypt an image. It's a fun way to understand how image data works and how simple algorithms can be applied visually.

---

## 📌 Features

- Encrypts images by shifting and inverting RGB pixel values
- Decrypts previously encrypted images using the reverse operation
- Accepts custom shift values
- Supports all common image formats (e.g. PNG, JPG)
- Preserves image dimensions and format

---

## 🔧 How It Works

The script uses the following encryption logic for each RGB pixel:

```python
new_pixel = (255 - original_value + shift) % 256
