# Python Installation

To install the latest stable version of Python on Ubuntu:

### 1. Update the package list:
```bash
sudo apt update
```

### 2. Add the deadsnakes PPA:
The deadsnakes PPA contains newer Python versions for Ubuntu. Run:
```bash
sudo add-apt-repository ppa:deadsnakes/ppa
```

### 3. Install Python:
Install the desired Python version:
```bash
sudo apt install python3.x
```
Replace `3.x` with the specific version number (e.g., `3.11`).

### 4. Verify the Installation:
Check if Python was installed successfully:
```bash
python3.x --version
```

### 5. (Optional) Set Python Version as Default:
If you want Python 3.x to be the default, configure the system’s `update-alternatives`:
```bash
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.x 1
```

Then select the version:
```bash
sudo update-alternatives --config python3
```

### 6. Install Python Distutils:
Python distutils is necessary for pip installation:
```bash
sudo apt-get install python3.x-distutils
```
