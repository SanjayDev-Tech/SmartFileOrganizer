# 📂 Smart File Organizer (Automated Directory Manager)

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Automation](https://img.shields.io/badge/Task-Automation-orange)](https://github.com/)

**Smart File Organizer** is a robust Python-based automation tool designed to keep your workspace clutter-free. It monitors a specified directory in real-time and automatically categorizes incoming files into dedicated folders based on their file extensions.



---

## 🚀 Key Features

* **Real-time Event Monitoring:** Leverages the `watchdog` API to listen for file system events (Creation/Modification), ensuring instant organization without manual triggers.
* **Intelligent Categorization:** Automatically sorts files into predefined categories:
    * 🖼️ **Images:** `.jpg`, `.png`, `.gif`, `.webp`
    * 📄 **Documents:** `.pdf`, `.docx`, `.txt`, `.xlsx`
    * 🎥 **Videos:** `.mp4`, `.mkv`, `.mov`
    * 🎵 **Music:** `.mp3`, `.wav`
    * 📦 **Archives:** `.zip`, `.rar`, `.7z`
* **Duplicate Handling:** Built-in logic to handle filename collisions by appending unique timestamps or counters to prevent data overwriting.
* **Lightweight & Fast:** Optimized using `os.scandir()` for low memory footprint and high performance.

---

## 🛠️ Technical Stack

* **Language:** Python 3.10+
* **Core Libraries:** * `watchdog`: For cross-platform file system event monitoring.
    * `shutil`: For high-level file operations (moving, copying).
    * `os`: For directory traversal and path manipulation.

---

## 📂 Project Structure

```text
SmartFileOrganizer/
├── main.py              # Main execution script & event handler
├── requirements.txt     # List of project dependencies
├── .gitignore           # Files to be ignored by Git (e.g., venv/)
└── README.md            # Project documentation

⚙️ Installation & Setup
1. Clone the Repository
Bash
git clone [https://github.com/YOUR_USERNAME/SmartFileOrganizer.git](https://github.com/YOUR_USERNAME/SmartFileOrganizer.git)
cd SmartFileOrganizer
2. Set Up Virtual Environment (Recommended)
Bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate
3. Install Dependencies
Bash
pip install -r requirements.txt
4. Configure Paths
Open main.py and update the source directory you want to monitor:

Python
WATCH_DIRECTORY = "C:/Users/YourName/Downloads"
5. Run the Organizer
Bash
python main.py
🛡️ License
This project is licensed under the MIT License - see the LICENSE file for details.

👨‍💻 Author
[sanjay Sharma] * [GitHub: @SanjayDev-Tech]

LinkedIn: [(https://www.linkedin.com/in/sanjay-sharma01/)]

Future Enhancements
[ ] Add a GUI for path selection.

[ ] Implement file compression for old documents.

[ ] Add MD5 checksum to identify exact duplicate files.
