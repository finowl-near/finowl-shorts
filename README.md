# 🦉 FinOwl Shorts – UX Design Specification

## 📱 Platform
- Web (responsive) + Mobile-first layout
- Integrated inside the main [FinOwl.finance](https://finowl.finance) app
- Built using Next.js (frontend), NEAR Wallet (auth/payment)

---

## 🔁 Navigation Structure

/shorts  

├── Explore Tab  

└── Generate Tab

---

## 🟣 1. EXPLORE TAB – Daily Videos Feed

### Purpose:
Showcase all FinOwl-generated crypto short videos in a TikTok-style feed. Encourage discovery and drive users to generate or trade.

### Components:

#### 🔝 Hero Section
- Title: `FinOwl Shorts – Daily Crypto in 30s`
- CTA: `[ 🎥 Generate My Video ]` → links to Generate tab

#### 🔍 Search & Filters
- Search bar: `Search token or ticker...`
- Filters: [Trending] [DeFi] [Meme] [ETH Ecosystem] [Custom]

#### 📺 Video Feed (Scrollable Cards or Grid)
Each card includes:
- Thumbnail (image or preview GIF)
- Title: "Why $SOL Is Pumping"
- Duration (e.g. ⏱ 0:30)
- Source: YouTube / TikTok
- CTA: `🔗 Trade with NEAR` (Intent URL)
- Option: `🔁 Remix This`

---

## 🟡 2. GENERATE TAB – Create a Custom Video

### Purpose:
Allow NEAR wallet users to pay and generate personalized AI crypto videos for specific tokens.

### Flow Steps:

#### 1️⃣ Choose Token
- Field: `Enter Token or Ticker`
- Autocomplete: e.g. `$ETH`, `$SOL`, `$GIGA`
- Option: `[ Use trending token ]` (from FinOwl trending API)

#### 2️⃣ Customize Video
- 🎙 Voice Style:
  - Options: Calm / Energetic / Comic / Robotic
- 🎨 Visual Style:
  - Options: Light / Dark / Meme / Dashboard
- 📝 Custom Prompt (optional):
  - Field: `Write something to emphasize (ex: whale activity, narrative)`
- 📄 Preview Block:
  - Displays combined prompt output:  
    `“Summarize $SOL’s treasury adoption, Kamino vaults, and low fees in 30s with light visuals and energetic narration.”`

#### 3️⃣ Pay with NEAR
- Wallet Connect Component
- Payment amount: `0.25 NEAR`
- Button: `[ ✅ Pay and Generate ]`
- Progress loader: `“Generating your video… (~1 min)”`

#### 4️⃣ Video Preview & Output
- Embedded player (MP4 or YouTube)
- Buttons:
  - `[ 📥 Download MP4 ]`
  - `[ 🔗 Share on X / TikTok ]`
  - `[ ♻️ Request Changes ]`
  - `[ 💹 Trade This Token ]`

---

## 🎨 Brand & Design Notes

- Fonts: FinOwl’s base typography
- Color Palette:
  - Background: Dark theme (`#0b0c10`, `#1e1f25`)
  - Accents: NEAR Purple, Bright Green, Gold Highlights
- Icons: Use consistent crypto and Web3 iconography
- Animations: Smooth transitions between steps (preferably GSAP or Tailwind Motion)
- Watermark: Include **FinOwl Shorts** logo in bottom-right corner of video thumbnails and previews

---

## 🧠 Optional Enhancements

- 🔔 Trending Tokens Banner above video feed
- 📁 "My Videos" tab to show user's generated history
- 🧪 Feedback modal after video generation (thumbs up/down + comment)

---

## ✅ Deliverables for Design

- Figma flow for:
  - **Explore Tab**
  - **Generate Tab**
- Desktop + Mobile responsive
- Reusable components:
  - Video Card
  - Prompt Form
  - NEAR Wallet Connect
  - CTA Buttons
  - Loading state

---

### 📌 Example User Story

> "A NEAR user logs in, sees that $HYPE is trending, clicks 'Generate My Video,' selects a comic voice style, adds a custom prompt, pays 0.25 NEAR, and receives a downloadable 30s video they can instantly post on TikTok and X. A 'Trade Now' button under the video lets others interact directly on-chain."

---

**FinOwl Shorts**  
*AI-generated crypto videos. Powered by NEAR.*

![image](https://github.com/user-attachments/assets/900aa527-209c-4fcb-8f00-adaa6d4e8f6a)
![image](https://github.com/user-attachments/assets/86fad508-d9cb-46c5-aa72-80a11b081160)

