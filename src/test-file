import requests, json, base64
from sempy.fabric import FabricRestClient

# --- SET THESE ---
WORKSPACE_ID = "YOUR_WORKSPACE_ID"
NOTEBOOK_NAME = "NB_from_github"
GITHUB_RAW_URL = "https://raw.githubusercontent.com/<user>/<repo>/<branch>/<path/to/file>.py"
# -----------------

# 1) download python file from GitHub
resp = requests.get(GITHUB_RAW_URL)
resp.raise_for_status()
py_code = resp.text
