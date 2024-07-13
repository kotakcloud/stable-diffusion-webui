## Installation
python3.10 -m venv .venv
source .venv/bin/activate
ARCHFLAGS="-arch x86_64" python3.10 -m pip install -r requirements.txt
ARCHFLAGS="-arch x86_64" sh webui.sh

## Running from second time onwards:
source .venv/bin/activate && ARCHFLAGS="-arch x86_64" sh webui.sh
// To remove memory limitations:

source .venv/bin/activate && ARCHFLAGS="-arch x86_64" PYTORCH_MPS_HIGH_WATERMARK_RATIO=0.0 sh webui.sh