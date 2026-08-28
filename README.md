# QR Generator

A simple Python application that generates a QR code from a user-provided URL and saves it as an image file.

---

## Features

* Generate QR codes instantly
* Converts URLs into QR codes
* Saves QR code as a PNG image
* Beginner-friendly Python project
* Simple console-based program

---

## Technologies Used

* Python 3
* `qrcode` library

---

## Requirements

Install the required library before running the program:

```bash id="f7d0k3"
pip install qrcode[pil]
```

---

## How the Program Works

1. The user enters a URL.
2. The program creates a QR code using the `qrcode` library.
3. The generated QR code is saved as an image file on the desktop.
4. A success message is displayed.

---

## Code Explanation

### Importing the Library

```python id="ssu2ca"
import qrcode
```

Imports the QR code generation library.

---

### Taking User Input

```python id="d8llst"
url = input("enter the url: ").strip()
```

Takes the URL input from the user and removes extra spaces.

---

### File Path

```python id="rtx0si"
file_path = "C:\\Users\\HP\\Desktop\\qrcode.png"
```

Specifies the location where the QR code image will be saved.

---

### Creating the QR Code

```python id="mylk6x"
qr = qrcode.QRCode()
qr.add_data(url)
```

Creates a QR code object and adds the entered URL data.

---

### Generating and Saving the Image

```python id="if7myq"
img = qr.make_image()
img.save(file_path)
```

Generates the QR image and saves it as a PNG file.

---

## Sample Output

```text id="ql0lxg"
enter the url: https://google.com
QR CODE IS GENERATED ON YOUR DESKTOP
```

---

## Advantages

* Fast QR code generation
* Easy to use
* Useful for sharing links quickly
* Lightweight and efficient

---

## Future Improvements

* Add custom file name support
* Create colored QR codes
* Build a graphical user interface (GUI)
* Generate QR codes for text, contact details, and WiFi passwords

---

## Author

* Project Name: **QR Generator**
* Language Used: **Python**
* BY DIPIKA ANAND
