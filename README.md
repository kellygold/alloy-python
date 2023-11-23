# Alloy Python SDK

This SDK provides a Python interface for interacting with Alloy APIs. It's designed for flexibility and easy integration into Python projects.

This package will be distributed via pypi and available via `pip install alloy-xxx`

## Installation

### Clone the repository

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/alloy_python.git
```

### Set up a virtual environment

Navigate to the cloned directory and create a virtual environment. This keeps dependencies required by this project separate from your global Python environment.

```bash
cd alloy_python
python -m venv venv
```

Activate the virtual environment:

- On macOS/Linux:
  ```bash
  source venv/bin/activate
  ```
- On Windows:
  ```bash
  venv\Scripts\activate
  ```

### Install dependencies and the package

Install the required dependencies and the SDK itself:

```bash
pip install -r requirements.txt
pip install .
```

## Usage

After installation, you can import and use the SDK in your Python projects. Initialize the `Embedded` class with your API key:

```python
from alloy_python import Embedded

# Initialize with your API key
embedded = Embedded("your_api_key_here")

# Example usage with the App class
response = embedded.App.get_apps()
print(response)

# Example usage with other classes
# response = embedded.User.get_user()
# response = embedded.Workflows.list()
# ... and so on
```

Replace `"your_api_key_here"` with your actual API key. The `Embedded` class provides access to all the features of the Alloy Python SDK.

## Contributing

Contributions to the SDK are welcome. Please ensure to follow the coding standards and write tests for new features.

## License

Specify the license under which your SDK is distributed.
