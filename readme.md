### Azure Functions Python Extension
- [How to author your first Python Extension](https://docs.microsoft.com/en-us/azure/azure-functions/author-python-worker-extensions)

### Usage to Example Function App
The _example/ folder contains a sample Function App that will use the python_worker_extension_timer. Ensure you have [Azure Functions Core Tools](https://github.com/Azure/azure-functions-core-tools) installed.
Please follow the steps below to validate the extension end to end:

1. Open a Windows PowerShell or any Linux shell as you prefer.
2. Change your directory into the `_example/`
3. Create a Python virtual environment by `py -m venv .venv` in Windows, or `python3 -m venv .venv` in Linux.
4. Activate the Python virutal environment with `.venv\Scripts\Activate.ps1` in Windows PowerShell or `source .venv/bin/activate` in Linux shell.
5. Install the packages for your function app project `pip install -r requirements.txt`
6. Start the function host with `func host start --verbose`

You should now be able to access `http://localhost:7071/api/HttpTrigger`. Each http response reports the time elapsed of request processing.
