# Sell.app Blacklister

Sell.app Blacklister is a Python script designed to manage and update blacklists using Sell.app API. It supports multi-threaded processing with proxy rotation for efficient operation.

## Features

- **API Integration:** Interacts with Sell.app API to fetch existing blacklisted items and add new ones.
- **Multi-threaded Processing:** Utilizes threading for concurrent domain processing, improving speed.
- **Proxy Support:** Rotates through a list of proxies to handle rate limits and network errors gracefully.
- **File Handling:** Reads domains and proxies from text files for easy configuration.

## Setup

### Prerequisites

- Python 3.x installed on your system.
- `pip` package manager to install Python dependencies.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/zayys-services/sellapp-blacklist.git
   cd sellapp-blacklist
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up Sell.app API key:**
   - Navigate to `config.json` and open it in a text editor.
   - Ensure your Sell.app API key has blacklist permissions.
   - Paste your Sell.app API key where it says `sell_app_api_key here`.

4. **Prepare domain and proxy files:**
   - Customize blacklists in the `data` folder and proxies in `data/proxies.txt` files as needed.

### Usage

Run the script using Python:

```bash
python main.py
```

Alternatively, you can run `start.bat` for automatic setup and execution.

### Notes

- Modify files in the `data` folder to update ASNs, Countries, Emails, IPs, Proxies, or Wildcard Emails.
- Ensure HTTP proxies are listed in `data/proxies.txt`.
- Initiate the script via `start.bat` or `python main.py`; `start.bat` automates module updates and Python installation.
- Monitor console output for real-time status updates and errors during execution.

## Contributing

Contributions are welcome! Fork the repository and submit pull requests for improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
