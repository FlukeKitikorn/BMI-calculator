# BMI Calculator

> [🇹🇭 ภาษาไทย](README.th.md)

A Body Mass Index (BMI) calculator application built with Python and Tkinter, featuring an intuitive and beautiful GUI.

## 📋 Features

- Calculate BMI from weight and height
- Display health assessment based on BMI value
  - Underweight: BMI 0-18.5
  - Normal: BMI 18.6-25
  - Overweight: BMI 25.1-30
  - Super overweight: BMI > 30
- Real-time height and weight adjustment with sliders
- Dynamic man image that scales with selected height
- Clean and user-friendly interface

## 🖼️ Screenshot

The application features a beautiful interface with icons and illustrations.

## 🛠️ Technologies Used

- **Python 3.x**
- **Tkinter** - GUI framework
- **Pillow (PIL)** - Image processing
- **PyInstaller** - Executable builder

## 📦 Installation

### Install Dependencies

```bash
pip install pillow
```

### Run the Application

```bash
python main.py
```

## 💻 Usage

1. Launch the BMI Calculator application
2. Adjust height (0-220 cm) using the left slider
3. Adjust weight (0-200 kg) using the right slider
4. Click "View Report" button to calculate
5. The application will display your BMI value and health assessment

## 📁 Project Structure

```
.
├── main.py                 # Main application file
├── main.spec              # PyInstaller configuration
├── image/                 # Image assets folder
│   ├── icon.png          # Application icon
│   ├── top.png           # Header image
│   ├── box.png           # Value display box
│   ├── scale.png         # Scale image
│   └── man.png           # Scalable man image
├── exe file/              # Executable files folder
│   ├── BMI calculator.exe
│   └── favicon.ico
└── build/                 # PyInstaller build folder
```

## 🔨 Building Executable

This project uses PyInstaller to create a Windows executable.

```bash
pyinstaller main.spec
```

Or build from scratch:

```bash
pyinstaller --onefile --windowed --icon=favicon.ico main.py
```

The generated .exe file will be in the `dist/` folder.

## 📝 BMI Formula

```
BMI = weight (kg) / (height (m))²
```

## ⚠️ Important Notes

- Ensure the `image/` folder and all image files are in the correct location
- The code references `Image/` (capital I) - verify this matches your actual folder name

## 📄 License

This project is free to use.

## 👨‍💻 Future Enhancements

Potential improvements:
- Add calculation history tracking
- Include BMI change graphs
- Multi-language support
- Daily calorie intake calculator
- Health recommendations based on results
