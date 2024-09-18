Keylogger using pynput
Overview
This is a basic Keylogger implemented in Python using the pynput library. The keylogger listens for keystrokes and logs them into a text file (log.txt). It captures both regular characters and special keys (like space, enter, etc.).

Features
Logs keystrokes in real time.
Captures both printable characters and special keys (e.g., space, enter).
Saves keystrokes in a file (log.txt).
How it Works
The program uses the pynput library’s Listener class to listen for keystrokes. When a key is pressed:

Regular keys: Are written directly to the log.txt file.
Special keys: Such as space and enter are handled separately to ensure they are logged in a readable format.
Code Explanation
The on_press() function is triggered every time a key is pressed.
The try-except block is used to differentiate between normal characters and special keys.
The Listener class starts listening to the keyboard events, and the program keeps running in the background until manually stopped.
Usage
Prerequisites
Python 3.x

Install the pynput library:

bash
Copy code
pip install pynput
How to Run
Clone this repository:

bash
Copy code
git clone <repository-url>
Run the keylogger script:

bash
Copy code
python keylogger.py
The keystrokes will be logged in a file named log.txt in the same directory as the script.

Warning
⚠️ Disclaimer: This project is for educational purposes only. Unauthorized use of keyloggers is illegal and unethical. Please use this responsibly.
