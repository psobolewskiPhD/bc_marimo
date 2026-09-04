# Batch Connect - marimo notebooks, fully sandboxed

This interactive app launches marimo using a uv container and everything is fully sandboxed to a single directory (created if it doesn't exist):  
- The uv package cache and virtual environments needs for Python code execution in notebooks are created in `/tmp` and are not retained between sessions. 
- The saved notebooks are retained in `marimo_notebooks` and will include PEP723 script metadata so that dependencies (pinned) can be reinstalled on-demand.
