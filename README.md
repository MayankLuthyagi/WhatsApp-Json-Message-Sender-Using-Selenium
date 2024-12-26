# WhatsApp-Json-Message-Sender-Using-Selenium

This Python-based project automates sending messages to WhatsApp communities using data stored in a JSON file. It is ideal for sending bulk updates, reminders, or notifications to multiple WhatsApp groups quickly and efficiently.

### Features:
- Automates WhatsApp messaging using Selenium WebDriver.
- Reads message details from a JSON file for bulk messaging.
- Easily customizable for different groups and messages.

---

### Prerequisites:

Before running the project, ensure that you have the following:

1. **Python 3.x** installed on your system.
2. **Google Chrome** browser installed.

---

### Installation and Setup:

1. **Clone the repository** to your local machine:

    ```bash
    git clone https://github.com/your-username/WhatsApp-Json-Message-Sender-Using-Selenium.git
    cd WhatsApp-Json-Message-Sender-Using-Selenium
    ```

2. **Install the required libraries**:

    Run the following command to install Selenium and the necessary dependencies:

    ```bash
    pip install selenium chromedriver-autoinstaller
    ```

    - **selenium**: For automating the web browser.
    - **chromedriver-autoinstaller**: To automatically download the correct version of `chromedriver` for your Chrome version.

3. **Fill in the required details** in the script (or follow the instructions below).

4. **Prepare the `file.json` with the necessary message data**.

    Example format for `file.json`:

    ```json
    {
      "messages":
        {
          "key1": "value1",
          "key2": "value2"
          "key3": "value3",
          "key4": "value4"
        }    
    }
    ```
    - `message`: The content of the message.

5. **Run the program** step by step:

    - Open the Python script `whatsapp_message_sender.py`.
    - You can run it line-by-line or as a full script.
    - The script will use the data from the `file.json` and automatically send messages to the corresponding WhatsApp groups.

---

### Step-by-Step Usage:

1. **Clone the repository**:

    ```bash
    git clone https://github.com/your-username/WhatsApp-Json-Message-Sender-Using-Selenium.git
    cd WhatsApp-Json-Message-Sender-Using-Selenium
    ```

2. **Install the dependencies**:

    ```bash
    pip install selenium chromedriver-autoinstaller
    ```

3. **Edit the `file.json`** with the message data (as shown above).

4. **Run the script**:

    ```bash
    python whatsapp_message_sender.py
    ```

    The program will:
    - Open WhatsApp Web using Selenium.
    - Log in to your WhatsApp account (you may need to scan the QR code if it's not already authenticated) I'm using options.add_argument(f"user-data-dir={user_data_dir}") to save the history on the chrome browser.
    - Send the message from the JSON file to group.

---

### Screenshot Examples:

1. **Details to be filled in the script** (Example):

   user_data_dir is important to save the history so next time you don't have to login on whatsapp
   
   ![image](https://github.com/user-attachments/assets/65d3fb0e-b1d4-4003-a631-e32a3ec476a6)


3. **Format for `file.json`**:
   ![image](https://github.com/user-attachments/assets/07a68f1a-1261-4521-bfd5-fd70612cba63)

---

### Troubleshooting:

- **Error while opening WhatsApp Web**: Ensure that you are logged in to WhatsApp Web on your browser before running the script.
- **No matching group name found**: Verify that the `group_name` in your code file matches exactly with the group name in WhatsApp (case-sensitive).
- **Chromedriver issues**: If you experience issues with ChromeDriver, run `chromedriver-autoinstaller` again to ensure the correct version is used.

---

### Contributing:

Feel free to contribute by forking the repository and submitting pull requests. You can suggest improvements, fix bugs, or add features. Please ensure that any contributions follow the coding standards and include relevant tests.
