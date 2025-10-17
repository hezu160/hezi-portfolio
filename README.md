AI-Powered Storybook Generator

> A complete AI-driven content pipeline that transforms a children's story text into a fully illustrated, comic-style visual story.

This project demonstrates a unique workflow combining AI-powered planning with Python-based web automation to automate creative content production.

---

## 🚀 How It Works

The process is a two-stage pipeline:

1.  **AI Planning Stage:**
    * A children's story is provided to a Large Language Model (LLM).
    * The LLM analyzes the narrative, breaks it down into distinct visual scenes, and generates a detailed, structured prompt for each scene, tailored for an image generation model. This showcases advanced **Prompt Engineering** skills.

2.  **Automation Execution Stage:**
    * A Python script takes the list of generated prompts.
    * It uses **Selenium** to automate a web browser, navigating to an online image generator.
    * For each prompt, the script programmatically inputs the text, clicks "Generate", waits for the image to be created, downloads the result, and saves it with a sequential filename.
    * The script includes a simple Tkinter GUI to show real-time progress.

### ✨ Key Features

* **Full End-to-End Automation:** From raw text to a complete set of downloadable images.
* **AI-Driven Content Strategy:** Leverages an LLM not just for text, but for visual direction and creating machine-readable instructions (prompts).
* **Robust Web Automation:** Uses Selenium's `WebDriverWait` for reliable interaction with dynamic web elements.
* **User-Friendly Progress:** A simple GUI provides feedback on the image generation progress.

---

## 🛠️ Technologies Used

* **Language:** Python
* **Core Libraries:**
    * `Selenium` - For browser automation and control.
    * `Tkinter` - For the real-time progress GUI.
    * `requests` - For downloading the generated images.
* **External Tools & Services:**
    * AI Chat Model (e.g., Gemini) - For the planning and prompt generation phase.
    * Web-based Image Generator (e.g., Stablecog) - As the target for automation.

---

## ⚙️ How to Use

1.  **Prerequisites:**
    * Python 3.x installed.
    * Google Chrome installed.
    * ChromeDriver compatible with your Chrome version.

2.  **Setup:**
    * Clone this repository.
    * Install the required libraries:
        ```bash
        pip install -r requirements.txt
        ```
    * Run Chrome in debugging mode from your terminal:
        ```bash
        "C:\Program Files\Google\Chrome\Application\chrome.exe" --remote-debugging-port=9222
        ```

3.  **Execution:**
    * Log in to your chosen image generator website in the debug-mode Chrome window.
    * Run the Python script:
        ```bash
        python main.py
        ```
    * The script will automatically open a new tab, navigate to the generator, and begin creating images from the predefined prompts.

---

*This project was developed as a personal exploration into building complete, AI-driven automation workflows.*
`
