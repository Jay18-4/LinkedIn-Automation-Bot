# LinkedIn Automation Bot

## Overview
This project is a Python-based bot built using Selenium to automate LinkedIn post engagement. It includes a feature to randomly select combinations of words from a JSON file, enabling customizable and unique comments for each interaction.

---

## Features
- Automates commenting on LinkedIn posts.
- Randomized comment generation using a JSON file to ensure unique responses.
- Simulates human-like behavior to avoid detection.
- Configurable to target specific posts or hashtags.

---

## Tools & Technologies
- **Python**: Core programming language.
- **Selenium**: For browser automation.
- **JSON**: To store and manage comment templates.
- **Chrome WebDriver**: To interact with the LinkedIn interface.

---

## How It Works
1. **Random Comment Generation**:
   - The bot reads from a JSON file containing predefined phrases.
   - It selects a random combination of words to generate natural-looking comments.

2. **Automation**:
   - Logs into LinkedIn using Selenium.
   - Finds posts based on hashtags or user input.
   - Posts generated comments on targeted posts.

---

### Using Cookies for Login
This bot simplifies the login process by saving cookies after you manually log in to LinkedIn. Here's how it works:

1. **Run the Script:**
   - When you run the bot for the first time, it opens the LinkedIn login page in your browser.

2. **Log in Manually:**
   - Enter your LinkedIn credentials and complete any required authentication (e.g., CAPTCHA or 2FA).

3. **Save Cookies:**
   - Once logged in, the script automatically saves the session cookies into a file (e.g., `cookies.json`) in the working directory. These cookies are used for subsequent runs, so you don't need to log in again manually.

4. **Avoid Sharing Cookies:**
   - Ensure that the `cookies.json` file is kept private and not uploaded to GitHub. Sharing this file could compromise your account security.

---

### **2. Do You Need `.gitignore`?**
If the cookie file is generated dynamically and isn’t uploaded to GitHub, you don’t necessarily need a `.gitignore`. However, including it is a good habit to avoid accidental uploads in the future.

#### **How to Add a `.gitignore` File**
1. Create a file named `.gitignore` in your repository's root folder.
2. Add the following line to the file:` linkedin_cookies.pkl`
3. Save the `.gitignore` file.

This ensures ` linkedin_cookies.pkl` won’t be uploaded, even if it’s accidentally added to your local Git repository.

---

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/Jay18-4/LinkedIn-Automation-Bot.git
   
## Prerequisites
- Download the ChromeDriver that matches your browser version from [ChromeDriver Downloads](https://chromedriver.chromium.org/downloads).
- Add the ChromeDriver executable to your system PATH or place it in the project directory.
