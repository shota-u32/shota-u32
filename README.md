- 👋 Hi, I’m @shota-u32
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
shota-u32/shota-u32 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import sqlite3
wallet_fpath = "/path/to/wallet/file.sqlite"
con = sqlite3.connect(wallet_fpath)
cur = con.cursor()
cur.execute("SELECT root FROM private_key")
key = cur.fetchone()[0]
