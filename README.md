# AI Assistant for Google Gemini

Quick AI queries using Google's Gemini API directly from Flow Launcher.

## Features
- 🌍 **Multilingual support** (English & Spanish)
- 🚀 **Multiple Gemini models** (Fast-lite, Flash, Pro-preview)
- ⚡ **Fast and direct responses** to your clipboard or editor
- 🔒 **Zero shell dependencies** for safe clipboard copying (No Command Injection)

## Requirements
- **Flow Launcher** installed
- **Python 3.8+**
- Python packages: `requests`, `python-dotenv`, `flowlauncher` (automatically installed or defined in requirements.txt)

---

## 📖 How to Use

Once the plugin is installed in Flow Launcher, you can interact with it using the default action keyword **`ai`**.

### 1. Configure your Google Gemini API Key
Before using the assistant, you need to set up your API Key (get one for free at [Google AI Studio](https://aistudio.google.com/)):
1. Open Flow Launcher.
2. Type:
   ```cmd
   ai setkey YOUR_GEMINI_API_KEY
   ```
3. Press **Enter** to confirm and save it.

### 2. Choose a Gemini Model
You can choose which model handles your requests:
1. Open Flow Launcher.
2. Type:
   ```cmd
   ai setmodel
   ```
3. Use the arrow keys to select a model (e.g., `gemini-2.5-flash-lite`, `gemini-2.5-flash`, or `gemini-3-pro-preview`) and press **Enter**.

### 3. Ask Gemini (Delimited Queries)
To perform a query, type your prompt and append **`||`** (two vertical bars) at the very end. The delimiter tells Flow Launcher you have finished typing and are ready to send the query.

**Examples:**
* Asking for a concept:
  ```cmd
  ai What is recursion? ||
  ```
* Asking for code (casing is fully preserved!):
  ```cmd
  ai Write a Python function using CamelCase naming ||
  ```

### 4. Actions on Response
Once Gemini returns the answer, you will see two options in Flow Launcher:
* **Open in Notepad**: Open the full response text inside a temporary Notepad file.
* **Copy to Clipboard**: Copy the answer directly to your clipboard securely.

---

## License
MIT