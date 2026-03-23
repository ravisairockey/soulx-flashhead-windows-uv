## 💻 UV (Unsolved Virtual) Install Guide for Windows  
*Authored by Amilgaul*

This guide shows how to install and run **SoulX-FlashHead** in a Windows environment using **UV** without Conda.

### 1. Install UV
```powershell
pip install uv
2. Create a virtual environment
uv venv flashhead --python 3.10
3. Activate the environment
flashhead\Scripts\activate
4. Install dependencies
uv pip install -r requirements.txt
5. Optional: Install FlashAttention and SageAttention
uv pip install ninja
uv pip install flash_attn==2.8.0.post2 --no-build-isolation
uv pip install sageattention==2.2.0 --no-build-isolation
6. Install FFmpeg (Windows-friendly)
uv pip install ffmpeg
✅ Notes
This guide avoids Conda entirely and uses UV for isolation.
Make sure you are running PowerShell as Administrator for system-wide installs if needed.
After this, you can run inference scripts inside the flashhead UV environment.
