git init
git config core.fileMode false
git config core.autocrlf true

echo "venv/", "__pycache__/", ".env", "*.log" | Out-File -FilePath .gitignore -Encoding utf8

echo "* text=auto" | Out-File -FilePath .gitattributes -Encoding utf8

git add .
git commit -m "Initial commit: Trading bot base with cross-platform config"

git branch -M main
git remote add origin https://github.com/Nishanthan15me104/trading_bot.git
git push -u origin main

