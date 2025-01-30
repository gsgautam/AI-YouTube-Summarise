Run n8n on localhost (Your Computer Only)
To start n8n on your local machine at http://localhost:5678, follow these steps:

✅ 1. Install n8n
If you haven’t installed n8n, install it using one of these methods:

🔹 Option 1: Install via npm (Recommended)
bash
Copy
Edit
npm install -g n8n
🔹 Option 2: Run n8n without installing (Temporary)
bash
Copy
Edit
npx n8n start
⚠️ This will not save workflows after restarting.

✅ 2. Start n8n
Run n8n on your local machine:

bash
Copy
Edit
n8n
or

bash
Copy
Edit
n8n start
n8n will now be available at:
👉 http://localhost:5678
✅ 3. Run n8n with Docker (Optional)
If you prefer using Docker:

bash
Copy
Edit
docker run -it --rm -p 5678:5678 -v ~/.n8n:/home/node/.n8n n8nio/n8n
Open http://localhost:5678 in your browser.
✅ 4. Keep n8n Running in the Background
To prevent n8n from stopping when you close the terminal:

Windows (PowerShell)
powershell
Copy
Edit
Start-Process -NoNewWindow -FilePath "n8n" -ArgumentList "start"
Mac/Linux (using nohup)
bash
Copy
Edit
nohup n8n > n8n.log 2>&1 &
