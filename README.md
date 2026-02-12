# Pixel Vault 🖼️📦
<img width="818" height="752" alt="Screenshot 1" src="https://github.com/user-attachments/assets/70fa79d0-70c0-4e20-bf88-db67330a5ad2" />

<img width="863" height="748" alt="Screenshot 2" src="https://github.com/user-attachments/assets/875c4920-dfa8-4005-bc0d-b195dfb15b90" />




I built this because I wanted to hide files inside images without messing up how the image looks. Most steganography tools tweak pixels and you can see the noise. Mine doesn't.

**Just drag, drop, and hide.**

---

## What is this exactly?

You take any image (PNG, JPG, doesn't matter) and any file (PDF, ZIP, another image, whatever). Pixel Vault stitches them together into one image file that:

- ✅ Opens normally in any image viewer
- ✅ Looks exactly like the original
- ✅ Contains your hidden file intact

Nobody can tell anything is there unless they know where to look.

---

## Wait, how?

Short version: Images have an "end of file" marker. Everything after that is ignored by image software. Pixel Vault just... puts your secret file after that marker. That's it.

Long version: I spent way too long reading PNG specifications at 2am so you don't have to.

---

## Why not the usual LSB method?

Because I tried it and:

- The image gets slightly discolored
- You can only hide small files
- It's slow as hell

Tail-end method = unlimited file size, zero quality loss, instant encoding.

---

## How to use it

**To hide a file:**

1. Pick a cover image
2. Pick the secret file
3. Click encode
4. You get a new image. Send it anywhere.

**To uncover the file:**

1. Drop the encoded image in
2. Click decode
3. Get your original file back

No servers. No accounts. No "upload to cloud." Everything happens in your browser tab.

---

## What can I hide?

Anything under like 2GB. I've hidden:

- Whole movies inside vacation photos
- A ZIP bomb inside a meme (don't do this)
- My password manager backup inside my dog picture

---

## Known quirks

- Some image hosts strip extra data. Discord is fine. Twitter is not. Test before you rely on it.
- If your image is 10MB and you hide a 100MB file, the result is 110MB. Physics.
- Gmail sometimes blocks these. Use WeTransfer-style links instead of attachments.

---

## Why did you make this?

Honestly? I thought it was cool that old BBS users did this in the 90s and nobody really does it anymore. Also I wanted to see if I could build something useful in just HTML/JS with zero dependencies.

Turns out I could.

---

## One more thing

If you actually use this for anything illegal, that's on you. I made it because steganography is fascinating, not so you can leak corporate secrets or whatever.

---

**Pixel Vault is free, open source, and always will be.**


## License

MIT
