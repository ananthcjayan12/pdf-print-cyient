# pdf_print_cyient

PDF Print Cyient is a scan-to-print workstation for uploading a master PDF, matching scanned serial numbers to the exact PDF page, previewing that page, and printing it through a local bridge.

## Project Structure

- `frontend/` - React/Vite web app.
- `print-server/` - Flask local print bridge and PDF page extraction service.
- `.github/workflows/` - Cloudflare Pages deploy and Windows bridge release builds.

## Local Start

Backend:

```bash
cd print-server
/opt/homebrew/bin/python3.12 -m venv .venv
.venv/bin/python -m pip install -r requirements.txt
.venv/bin/python app.py
```

Frontend:

```bash
cd frontend
npm install
npm run dev
```
