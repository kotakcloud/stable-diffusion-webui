python3.10 -m venv .venv
source .venv/bin/activate
ARCHFLAGS="-arch x86_64" python3.10 -m pip install -r requirements.txt
ARCHFLAGS="-arch x86_64" sh webui.sh