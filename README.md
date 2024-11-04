# EM|Panel
## Nginx and MySQL CLI Management Panel

###### This project was inspired by the XAMPP control panel, aiming to provide similar ease of use for managing an EMP stack (Nginx, MySQL, PHP) via a Ruby or Python-based interface.

This CLI management panel provides a simple interface for controlling Nginx and MySQL services, with support for starting, stopping, checking the status, and monitoring logs. The script is available in both Ruby and Python versions, allowing users to choose their preferred language for the same set of functions.

## Features

- **Start Services**: Enable and start Nginx and MySQL services.
- **Stop Services**: Stop and disable Nginx and MySQL services.
- **Check Configuration**: Verify Nginx configuration files.
- **Check Service Status**: Display the status of Nginx and MySQL services.
- **Monitor Logs**: Continuously monitor access and error logs for Nginx.

## Requirements

- **Ruby** (version 2.5 or higher recommended) **or Python** (version 3.6 or higher recommended)
- `sudo` privileges to manage services
- Nginx, MySQL, and multitail installed on your system

## Installation

1. **Clone the Repository** (or copy the script to your desired location):
   ```bash
   git clone https://github.com/88saiba/emp.git
   cd emp
   ```

2. **Ensure Nginx and MySQL are installed**:
   Follow the instructions for your specific OS to install Nginx and MySQL.

3. **Choose a Version and Run the Script**:

   ### Ruby Version:
   Run the Ruby script using the following command:
   ```bash
   ruby emp.rb
   ```

   ### Python Version:
   Alternatively, run the Python script with:
   ```bash
   python3 emp.py
   ```

## Usage

Once the script is running, you will see the following menu:

```
+===========+
Nginx, Mysql Panel
-------------
EMP-Menu
+===========+
1. Turn On Engine
2. Turn Off Engine
3. Check Preps
4. Check Engine
5. View Logs
0. Bail Out
-------------
Always press 'q' to back menu
+===========+
```

### Options

- **1**: Start Nginx and MySQL services.
- **2**: Stop Nginx and MySQL services.
- **3**: Check Nginx configuration files.
- **4**: Check the status of Nginx and MySQL services.
- **5**: Monitor Nginx access and error logs.
- **0**: Exit the program.

### Navigation

- Press the corresponding number to select an option.
- To return to the main menu from sub-options, press `'q'`.

## Easy Access

For faster access to the management panel, set up an alias in your shell profile (e.g., `.bashrc` or `.zshrc`). Add the following line, replacing `/path/to/` with the actual path to your chosen version:

#### if you prefer Ruby
```bash
alias empanel="ruby /path/to/emp.rb"
```

#### or, if you prefer Python
```bash
alias empanel="python3 /path/to/emp.py"
```

After adding the alias, reload your shell profile:

```bash
source ~/.bashrc   # or source ~/.zshrc
```

Now you can start the panel by simply typing:

```bash
empanel
```

## Notes

- If you encounter any issues, ensure that you have the necessary permissions to manage the services and that Nginx and MySQL are correctly installed.
- The scripts assume you are running them in a Unix-like environment (Linux/Mac).
- If you have a different server or relational database management system (RDBMS), feel free to modify the commands within this program’s script. Think of this as just a skeleton with the base logic in place.

## License

This project is licensed under the [MIT License](LICENSE).
