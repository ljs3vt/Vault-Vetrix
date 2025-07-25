# 🔐 Secure SSH Access Instructions

Welcome! To access the server, you'll use secure SSH key authentication. This guide walks you through the setup process. **Before getting started, please contact me directly to receive access approval and a server IP address.**

---

## 📩 Step 1: Contact Me First

Before continuing, please **contact me** to request access.

> 📬 **Email:** loganvt@proton.me  
> 📱 **Discord (recommended):** @koala_trash

Once approved, I will provide you with:
- The server IP address
- A username for login
- Any specific port information (if not using default port 22)

---

## 🛠️ Step 2: Generate Your SSH Key

If you don't already have an SSH key:

### On Windows:
1. Download & Install FileZilla (Client) from this link:
   https://filezilla-project.org/
   
2. Download & Install PuTTYgenfrom this link:
   https://puttygen.com/

3. Creating Private & Public key:
   In PuTTYgen, Select ED25519 key (4th checkbox at the bottom)
   
   Follow steps shown on PuTTYgen to generate
   
   After generation click (Save Private Key) place it somewhere safe (DO NOT DELETE IT)
   
   Copy Content in text box above Generate & send it to me
   
   I will contact you when your key is added to server

5.  Setting up FileZilla:
    Open FileZilla

    Go to File → Site Manager

    Add a new entry with:

        Protocol: SFTP - SSH File Transfer Protocol

        Host: your server’s IP or domain

        Port: 22 (or whatever SSH port you use)

        Logon Type: Key file

        User: jesse

        Key file: browse to and select id_ed25519.ppk (private key)
   
### On Linux/macOS:

```bash
ssh-keygen -t ed25519 -C "your_user@server_ip"
```

**Send me the public key (`id_ed25519.pub`) — _NOT_ the private key (`id_ed25519`)!**

 I will contact you when your key is added to server


##**✅️ All Done!**