# Google Translate for GoldenDict

A lightweight Google Translate script that integrates with **GoldenDict** to translate words and phrases with a simple **Ctrl + C + C** shortcut (modifiable).

## Features
- **Instant Translation**: Uses Google Translate API to provide quick translations.
- **Customizable Shortcut**: Works with **GoldenDict's External Programs** feature (default: `Ctrl + C + C`).
- **Multi-language Support**: Translate between different languages easily.
- **Automatic Source Language Detection**: The script automatically detects the source language.
- **Set Target Language**: You can specify the target language for translations.
- **No API Key Needed**: Uses Google’s public translation endpoint.

## Installation

### 1. Install Dependencies
This script requires **Python 3** and `beautifulsoup4`.

```bash
pip install beautifulsoup4 requests
```

### 2. Clone the Repository
```bash
git clone https://github.com/farzadhallaji/GoogleTranslateforGoldenDict.git
cd GoogleTranslateforGoldenDict
```

### 3. Make the Script Executable
```bash
chmod +x google_translate.py
```

### 4. Configure GoldenDict
1. Open **GoldenDict** and go to `Edit > Dictionaries`.
2. Navigate to the **"Programs"** tab and click **"Add"**.
3. Set the following options:
   - **Command Line:**  
     ```
     python /path/to/google_translate.py en %GDWORD%
     ```
   - **Working Directory:** `/path/to/script/`
   - **Input Format:** Plain Text
   - **Output Format:** HTML (or Plain Text)

4. Click **OK**, then **Apply**.

### 5. Test the Script
- Restart **GoldenDict**.
- Select a word in any application and press **Ctrl + C + C**.
- The translation should appear in **GoldenDict**.

## Usage
Run manually in the terminal:
```bash
python google_translate.py en "hello world"
```
Or use **GoldenDict** for instant lookup.

## Customization
- Modify the shortcut in **GoldenDict settings**.
- Change the **default language** by editing the script’s `target_language`.
- You can translate to multiple languages by changing the target language parameter.

## License
MIT License. Free to use and modify.

---
Contributions welcome!

