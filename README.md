# INSTRUCTIONS (Read till bottom, all steps are extremely crucial and are unavoidable)

-----

# ⚠️ NOTE: ONLY RUNS ON MACOS

-----

## 💻 AuroraGeneLab Setup Guide for macOS (Bash Instructions)

This guide provides the complete procedure to acquire both the source code and the compiled application, organize them into the required **`AuroraGeneLab`** folder, and launch the **Aurora AstroBio Navigators** app.

-----

### **Part 0: Install Homebrew and Node.js (Prerequisites)**

The proxy server requires **Node.js** to run, and the best way to install Node.js on a Mac is by using the package manager **Homebrew**.

1.  **Open your Terminal** application.

2.  **Install Homebrew** (if you don't have it):

    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

    *Follow the on-screen instructions, which may include entering your password.*

3.  **Install Node.js** (includes npm) using Homebrew:

    ```bash
    brew install node
    ```

-----

### **Part 1: Initial Setup and Cloning (Terminal Commands)**

These commands will create the main project folder on your Desktop and clone the source code repository into it.

1.  **Navigate to the Desktop directory:**

    ```bash
    cd ~/Desktop/
    ```

2.  **Execute the following setup commands** one by one:

    ```bash
    # 1. Create the main project directory named AuroraGeneLab
    mkdir AuroraGeneLab

    # 2. Navigate into the new directory
    cd AuroraGeneLab

    # 3. Clone the Aurora_AstroBio_Navigators source code
    git clone https://github.com/Codemaster-AR/Aurora_AstroBio_Navigators.git
    ```

After running these commands, the source code will be located in **`~/Desktop/AuroraGeneLab/Aurora_AstroBio_Navigators/`**.

-----

### **Part 2: Set up the Node.js Proxy Dependencies**

The proxy server (`proxy.js`) is required to handle network requests for the main application. You must install its dependencies first.

1.  **Navigate to the Source Code Directory:**
    Open your Terminal and make sure you are in the folder containing `proxy.js` (which is inside the cloned repo):

    ```bash
    cd ~/Desktop/AuroraGeneLab/Aurora_AstroBio_Navigators/
    ```

2.  **Install the 'express' dependency:**
    The proxy requires the **Express** framework to run. Use Node Package Manager (npm) to install it:

    ```bash
    npm install express
    ```

-----

### **Part 3: Download the Application (Manual)**

The executable application must be downloaded separately from the web and placed directly inside the main setup folder.

1.  **Visit the Download URL:**
    Open your web browser and navigate to the application download page:
    [https://aurora-astrobio-app-download.w3spaces.com/](https://aurora-astrobio-app-download.w3spaces.com/)

2.  **Download the App:**
    Click the appropriate link or button on the website to download the application package (this will typically be a `.dmg` or `.zip` file).

3.  **Move the File:**
    Move the downloaded file from your Downloads folder directly into the **`~/Desktop/AuroraGeneLab`** folder.

-----

### **Part 4: Run the Proxy and Launch the Main Application**

With all files downloaded and dependencies installed, you can now run the proxy and launch the main app.

1.  **Run the Proxy Server:**
    If you are still in the **`Aurora_AstroBio_Navigators/`** folder from Part 2, start the proxy server using Node.js:

    ```bash
    node proxy.js
    ```

    The proxy server will now be running and listening for connections. **Keep this Terminal window open** while you use the main application.

2.  **Launch the Application:**
    Navigate to your **Desktop** and open the **`AuroraGeneLab`** folder.

      * **Double-click** the downloaded application file (the `.dmg` or `.app` file) inside the `AuroraGeneLab` folder to install or run the **Aurora AstroBio Navigators** application.

### **Make sure the terminal app is running at all times for the proxy to work and connect!**
### **All data is live and has a real-time connection with NASA OSRDR!**





-----

## ⚠️ **CRITICAL WARNING: MANUAL REPEAT REQUIRED\!** ⚠️

-----

> \*\*After your Mac opens from a restart or if the terminal application was quit, you must follow the following commands in the given order for the app to fucntion and connect properly, this is live data:
>
> ```bash
> cd ~/Desktop/AuroraGeneLab/Aurora_AstroBio_Navigators/
> node proxy.js
> 
> ```
> 
>
> **This double execution is a known, required configuration step. Skipping this will cause a setup failure.**

---
