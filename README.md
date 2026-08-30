# 🍪 OB2 Cookie Edition

A **cookies-only** edition of [OpenBullet 2](https://github.com/openbullet/OpenBullet2) — built for checking cookies against web apps you **own or are authorized to test**.

It keeps the full OpenBullet 2 engine and interface, but replaces the credential/combo workflow with a cookie-first one: load cookie files, inject them into requests, and validate them.

**Cookie Edition by [Mrx001](https://t.me/+1Dn5wvGgeMwxMzcx)** · Telegram channel: **https://t.me/+1Dn5wvGgeMwxMzcx**

---

## ✨ What's different from normal OpenBullet 2

- **Cookies wordlist type** — each line is a **path to a cookie file** (Netscape `.txt`, JSON export, or a header string).
- **Load a whole cookies folder** — *Cookies → Add → Load cookies folder* picks a folder and turns every cookie file into one wordlist.
- **Cookie blocks** in the Stacker:
  - **Cookie Container** — loads the cookies into the request jar and returns them in header format (`COK`).
  - **Cookie Netscape** — returns the cookies in Netscape `cookies.txt` format (`COOKIENETSCAPE`).
  - **Inject Cookies** — just loads the cookies into the jar (no output).
- New configs start ready-to-go with a Cookie Container block, so cookies flow out of the box.
- Cookie-flavored branding and the **`.mrx`** config format.

---

## 📥 Download & run (Native / Windows)

1. Go to the [**Releases**](../../releases) page and download **`OB2-Cookie-Edition-Native.zip`**.
2. Extract it anywhere.
3. Run **`OpenBullet2.Native.exe`**.

> Requires the **[.NET 10 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/10.0)** (Windows). Do **not** run as Administrator.

---

## 🧪 Sample config — `test.mrx`

This repo includes **`test.mrx`** (also pre-loaded in the app under **Configs → Test - Cookie Check**). It shows the basic cookie flow. To use it:

1. **Cookies → Add → Load cookies folder** → pick a folder of cookie files.
2. **Jobs** → create a Multi Run job → pick the **Test - Cookie Check** config and your cookies wordlist.
3. To fully validate, open the config's **Stacker** and add an **HTTP Request** block (your target) followed by a **Keycheck** block that marks SUCCESS / FAIL from the response.

---

## 💜 Support / Donate

If this project is useful to you, donations are appreciated (but never required). Please **double-check the address** before sending — transactions can't be reversed.

| Coin | Network | Address |
| --- | --- | --- |
| **USDT** | TRC20 | `TPa5r3fAWKAA6FTeitbSXegdcW8qb5FUUW` |
| **BTC** | Bitcoin | `1Cg8ejN4gErgjMc6gTh6HQvEpZ4xRWpcaM` |
| **ETH / USDT** | ERC20 | `0x84382d8107a901723f7e1c8e713a7f5837f86128` |
| **LTC** | Litecoin | `LL8xAWo9iSA3qeQr7VZX4q73jsDykMZJZk` |

Thank you for the support! 🙏

---

## ⚠️ Legal / disclaimer

**For authorized testing only.** Only test cookies on sites you **own** or have **explicit written permission** to test. Performing attacks or testing on systems you don't control is **illegal**. The author is not responsible for misuse.

---

## 📄 License & credits

Licensed under the **MIT License** (see [LICENSE](LICENSE)).

Based on **[OpenBullet 2](https://github.com/openbullet/OpenBullet2)** by **Ruri** and contributors. This is an independent, community fork.
