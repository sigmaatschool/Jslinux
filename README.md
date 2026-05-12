# Jslinux

Static demo for v86-based Linux in the browser.

## Netlify deployment

- Publish directory: `.` (project root)
- No build command required
- Keep `index.html`, `public/libv86.js`, `v86.wasm`, and `seabios.bin` in the repo
- The site now boots from a local ISO/disk image uploaded in the browser
- OS internet access is enabled through a v86 network relay proxy
- The relay WSS endpoint can be changed directly in the site before booting
- No external CDN assets or remote OS images are required

## Using the demo

1. Open the site in your browser.
2. Choose a local `.iso`, `.img`, or `.bin` file using the upload control.
3. Click `Boot local image`.

## Notes

- This setup avoids remote asset loading so it works on networks that block CDNs.
- If you need a specific OS image, upload that file from your local machine instead of relying on an externally hosted ISO.
