2. “Restart & start coding” ka exact routine (every time)
   Step A: VS Code open

VS Code → Open Folder → materials-ml

Step B: Terminal me venv activate (recommended habit)

Windows PowerShell:

.\.venv\Scripts\Activate.ps1

Step C: Notebook open + kernel verify

Notebook open

Top-right kernel should be your .venv / “Python (materials-ml)”

Agar change ho gaya ho: Select Kernel → Python environment → .venv

Step D: Quick sanity cell (optional but fast)

First cell:

import sys
print(sys.executable)

✅ Path .venv ka aaye.

3. requirements.txt bana dein (one-time)

Terminal (venv activated):

pip freeze > requirements.txt

Agar future me project kisi aur machine par run karna ho:

pip install -r requirements.txt
