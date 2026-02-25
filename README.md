# Modified Whatsapp-API
<p align='center'>
  <img src="https://files.catbox.moe/rhm9rt.webp" width="172">
</p>

--- 

## Installation
```bash
npm install @ikhsan-project/dizzanzz
Usage
javascript
const {
  default: makeWASocket,
  // Other Options 
} = require('@ikhsan-project/dizzanzz');
How To Connect To Whatsapp
With QR Code
javascript
const {
  default: makeWASocket
} = require('@ikhsan-project/dizzanzz');

const client = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.00.1'],
  printQRInTerminal: true
})
Connect With Number
javascript
const {
  default: makeWASocket,
  fetchLatestWAWebVersion
} = require('@ikhsan-project/dizzanzz');

const client = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.00.1'],
  printQRInTerminal: false,
  version: fetchLatestWAWebVersion()
  // Other options
});

const number = "628XXXXX";
const code = await client.requestPairingCode(number.trim());

console.log("Your pairing code: " + code);
📦 Repository
GitHub: ikhsan135/bail-dizzanzz

text

## 🚀 **Langkah-langkah Publikasi**

```bash
# 1. Hapus direktori node_modules dan file lock (bersih-bersih)
rm -rf node_modules package-lock.json yarn.lock

# 2. Install dependencies
npm install

# 3. Build project
npm run build:tsc

# 4. Login ke npm (pastikan sudah punya akun)
npm login

# 5. Cek apakah nama package sudah tersedia
npm view @ikhsan-project/dizzanzz
# Jika error 404, berarti nama tersedia

# 6. Publish ke npm
npm publish --access public

# 7. Verifikasi
npm view @ikhsan-project/dizzanzz
