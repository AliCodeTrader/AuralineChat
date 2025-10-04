
# AuralineChat

A modern, liquid‑glass chat UI — sleek, artistic, and system‑aware (Light/Dark). Built with **Next.js + React + Tailwind** and crafted for real apps, demos, and design explorations.

> Lume = lumen (light). LumeChat is all about luminous glass, soft gradients, and delightful micro‑interactions.

---

## ✨ Features

- **Liquid‑Glass Aesthetic**: layered blur, subtle gloss, gradient halos, soft shadows.
- **System Theming**: fully adaptive **Light/Dark** via `prefers-color-scheme` + `dark:` variants.
- **Hero + Glass Dock**: polished landing with a floating glass dock (Start Chat / GitHub / LinkedIn / Version).
- **Chat Experience**
  - Bubbled messages with **grouping**, timestamps, and **read receipts** (sent → delivered → seen).
  - **Smart Scroll**: sticky top gradient, “**New messages**” pill, **Jump to Latest** button.
  - **Typing Indicator** with animated dots.
  - **Quick Replies** for instant demo interactions.
  - **Reactions** (👍🔥😂❤️😮) with hover toolbar + selected reaction badge.
  - **Attachments**: drag‑and‑drop / paste / picker (image preview + remove).
  - **Input**: textarea **auto‑resize**, Enter=send / Shift+Enter=new line.
  - **Command Palette** (**⌘K / Ctrl+K**): modal with glass UI, ready for action wiring.
- **Performance‑friendly**: no heavy libs; all effects with Tailwind + lightweight React code.
- **Accessibility**: focus styles, high‑contrast text, keyboard shortcuts, reduced motion friendly.

---

## 🧱 Tech Stack

- **Next.js (App Router)**
- **React 18**
- **Tailwind CSS** (no custom config required)
- **TypeScript** (recommended)

---

## 🚀 Getting Started

```bash
# 1) Install dependencies
pnpm install    # or: npm install / yarn

# 2) Run the dev server
pnpm dev        # http://localhost:3000

# 3) Build for production
pnpm build && pnpm start
```

> Requires Node 18+.

---

## 📂 Project Structure (key parts)

```
src/
  app/
    layout.tsx          # Global layout: gradients, blobs, system theming
    page.tsx            # Landing (Hero + Preview + Theming + Glass Dock)
    chat/
      page.tsx          # The LumeChat experience (all chat features)
  styles/
    globals.css         # Tailwind + base styles
```

---

## 🎮 Keyboard & UX

- **Enter** → Send message  
- **Shift + Enter** → New line  
- **⌘K / Ctrl+K** → Open Command Palette  
- **Esc** → Close Command Palette  
- **Drag & Drop / Paste** → Add image attachments in the input bar

---

## 🧪 Implementation Notes

- Reactions and receipts are **demo‑state** only (client‑side).  
  Wire them to your backend or sockets as needed.
- Attachments are previewed with `URL.createObjectURL` and **not uploaded** by default.
- Smart scroll uses a simple bottom‑proximity check; change the threshold to taste.
- Theming uses Tailwind `dark:` and system `prefers-color-scheme` — no extra plugin.

---

## 🗺️ Roadmap Ideas

- Real‑time via WebSocket (presence, typing, receipts)
- Search across messages + in‑palette actions
- Message actions: copy, edit, delete, pin
- File types: audio recorder + voice notes (waveform), PDF/doc previews
- Lightbox for media & galleries
- i18n (RTL/LTR), user mentions, code blocks with copy
- Unit tests for core UX behaviors

---

## 🖼️ Screenshots (placeholders)

> Replace with your own captures

```
/public/preview-landing.png
/public/preview-chat-light.png
/public/preview-chat-dark.png
```

---

## 🔗 Naming & Branding

**LumeChat** = luminous chat. Use soft violet ↔ cyan gradients and subtle glass rings.  
Fonts: modern, geometric; icons minimal; motion gentle.

---

## 📜 License

MIT — do whatever you want, just keep the copyright notice.

---

## 🙌 Credits

Designed & built with care. Inspired by glass morphism, premium OS UIs, and thoughtful micro‑interactions.
