# Privacy Shield - Desktop Screen Privacy Utility

Privacy Shield is a lightweight, modern, and user-friendly desktop application built with Python and PyQt6. It allows you to protect your privacy by placing overlay masks (rectangles or circles) over sensitive portions of your screen. 

Additionally, it comes with a **built-in mobile remote control web application** so you can manage your screen privacy overlays from your phone.

---

## Features

1. **Multiple Mask Shapes**: Supports both Rectangles and Circles.
2. **Dynamic Opacity**: Adjust transparency seamlessly from 10% to 100%.
3. **Move & Resize**: Drag masks anywhere on the screen or resize them using the bottom-right corner handles.
4. **Color Customization**: Easily toggle masks between **Black** and **White**.
5. **Border Control**: Toggle active selection outlines and resizing handles on or off so the mask blends seamlessly with your screen.
6. **Keyboard Shortcuts**: Use the global hotkey `Ctrl + Alt + H` from anywhere on Windows to quickly hide or show all active masks.
7. **Mobile Remote Control**: Scans your local network and displays a QR code to let you control everything from any smartphone or tablet.

---

## Installation & Setup

### Prerequisites
- Python 3.8 or higher installed on your system.

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
   cd YOUR_REPOSITORY
   ```

2. **Create and Activate a Virtual Environment**:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r screen_privacy_app/requirements.txt
   ```

4. **Run the Application**:
   - Double-click the `run_privacy_app.bat` file.
   - Or run directly from your terminal:
     ```bash
     python screen_privacy_app/main.py
     ```

---

## Remote Control Usage
When the application starts, it hosts a local web server (FastAPI) on port `8000` and displays a QR Code in your terminal.
1. Connect your phone and PC to the **same Wi-Fi network**.
2. Scan the QR code with your phone camera or enter the URL shown in the console.
3. Use the remote control dashboard to toggle opacity, change shapes, add/delete masks, switch colors, or hide active overlays completely!

---

## Technologies Used
- **PyQt6** for native desktop GUI, overlays, and system window control.
- **FastAPI & Uvicorn** for the mobile remote API server.
- **HTML/CSS/JS** for the mobile remote interface.
- **qrcode** for local CLI QR Code generation.
- **keyboard** for global Windows hotkeys.
