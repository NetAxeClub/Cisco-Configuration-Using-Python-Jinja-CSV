# Generate Cisco Configuration Template Using Python, Jinja2, and CSV

This program is designed to generate a configuration template for Cisco Catalyst/Nexus switches.

## Table of Contents

1. [Requirements](#1-requirements)
2. [Installation](#2-installation)
3. [Getting Started](#3-getting-started)
4. [Usage](#4-usage)
5. [Preview](#5-preview)
6. [Helpful Tips](#6-helpful-tips)
7. [TODOs](#7-todos)

---

### 1. Requirements

1. [Python @3.9.4](https://www.python.org/)
2. [Jinja2 @2.11.3](https://jinja.palletsprojects.com/en/2.11.x/)
3. [Visual Studio Code](https://code.visualstudio.com/) (Optional but strongly recommended)
4. [Cisco IOS Syntax](https://marketplace.visualstudio.com/items?itemName=jamiewoodio.cisco) (Extension for Cisco IOS Syntax Highlighting)

---

### 2. Installation

```python3
pip install -r requirements.txt
```

---

### 3. Getting Started

In the `CSV` directory, you can find four `.csv` files:

1. `01. params.csv`
2. `02. vlans.csv`
3. `03. etherchannels.csv`
4. `04. port_mapping.csv`

---

### 4. Usage

1. Open each `.csv` file _respectively_, and add the configurations that meet your needs. _(The csv files are populated with a sample configuration already)_
2. Open Visual Studio Code.
3. Open the Terminal within VSCode (`` Ctrl+` ``).
4. Run `python cisco_config_generator.py`.

Voila :sparkles:! Your configuration will automagically open in the default text editor.

**All generated configuration files are stored in the `configs` directory.**

> If the `.ios` file extension is not associated with any text editor on your machine, please associate it with VSCode.

---

### 5. Preview

![Preview](assets/preview.png)

---

### 6. Helpful Tips

1. Validate the generated configuration template before pasting it on your device.
2. **DO NOT** copy/paste the whole configuration all at once on your device. Divide the configuration template into sections.
3. Always save your configuration with `copy running-config startup-config` command. [Why?!](https://networkengineering.stackexchange.com/questions/52309/diffrence-between-wr-and-copy-running-config-to-startup-config#answer-52310)

---

### 7. TODOs

- [ ] Validate input fields in CSV files.
