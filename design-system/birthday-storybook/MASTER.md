# DESIGN SYSTEM MASTER — Birthday Cartoon Storybook & Toy Blind Box

## 1. Visual Direction & Style Fusion
- **Primary Style**: **Illustrated Cartoon Pop × Tactile Claymorphism & Comic Zine** (referencing `ui-ux-pro-max` Styles #9 *Claymorphism* & #38 *Neubrutalism / Illustrated Pop*).
- **Vibe**: Hand-crafted Sanrio / Pop Mart illustrated picture book, chunky 3D cartoon toys, thick comic ink outlines (`3px solid #2B1638`), hard offset cartoon shadows (`5px 5px 0px #2B1638`), tactile physical stickers, speech bubbles, and lively animated SVG cartoon characters.
- **Anti-Patterns Strictly Forbidden**:
  - ❌ NO dark-mode AI purple/pink neon gradients (`radial-gradient` on `#170722`).
  - ❌ NO generic glassmorphism (`backdrop-filter: blur` translucent dark cards).
  - ❌ NO system emojis (`👑`, `🧋`, `🍓`, `🌸`, `🎤`, `🎂`) anywhere in UI or content — 100% custom hand-drawn SVG vector illustrations and icons with consistent `2.5px–3px` ink strokes.

## 2. Color Tokens (Warm Pastel Pink & Lilac Cartoon Palette)
- `--bg-paper`: `#FFFDF7` (Warm Creamy Sketchbook Paper)
- `--bg-polka`: `#FCE7F3` / `#F3E8FF` subtle illustrated dot pattern
- `--ink`: `#2B1638` (Deep Plum-Charcoal Comic Ink — Contrast > 11:1 on `#FFFDF7`)
- `--ink-soft`: `#5E3B73` (Muted Berry Ink — Contrast > 5.8:1 on `#FFFDF7`)
- `--pink-pop`: `#FF6B9E` (Strawberry Milk Cartoon Pink)
- `--pink-pastel`: `#FFD1E3` (Cotton Candy Blush)
- `--lilac-pop`: `#A855F7` (Grape Soda Violet)
- `--lilac-pastel`: `#E9D5FF` (Taro Milk Tea Lavender)
- `--butter-yellow`: `#FFE066` (Comic Starburst Yellow)
- `--mint-cream`: `#B8F2E6` (Pastel Mint Sticker Accent)
- `--border-ink`: `3px solid #2B1638`
- `--shadow-toon`: `5px 5px 0px #2B1638`
- `--shadow-toon-sm`: `3px 3px 0px #2B1638`
- `--shadow-clay`: `inset -3px -4px 8px rgba(43, 22, 56, 0.12), inset 3px 4px 8px rgba(255, 255, 255, 0.8), 5px 5px 0px #2B1638`

## 3. Typography (`ui-ux-pro-max` Playful Cartoon Pairing)
- **Display / Headings**: `'Baloo 2'`, `'Fredoka'`, cursive/sans-serif (Weight 700–800, chunky rounded cartoon lettering with 3D ink extrusion shadow).
- **Handwritten / Comic Speech Bubbles & Notes**: `'Playpen Sans'`, cursive (Weight 500–700, authentic hand-drawn comic book feel).
- **UI & Body**: `'Nunito'`, sans-serif (Weight 600–800, high legibility).

## 4. Bespoke Animated SVG Characters & Interactive Mechanics
1. **Chibi Mascot "Bé Thỏ Taro & Mèo Dâu Tây"**: Animated SVG cartoon mascot with blinking eyes, wiggling ears, floating heart doodles, and expressive poses in every chapter.
2. **Chapter 1 — Illustrated Comic Magazine Cover (`BIRTHDAY TOON ZINE`)**:
   - Looks like a real illustrated Japanese/Korean Pop-Art Comic Zine cover with die-cut stickers, speech bubbles, a cartoon Chibi Princess illustration (or photo inside a cartoon sticker frame), and a physical supermarket barcode scanner gun sound + illustrated receipt!
3. **Chapter 2 — "Máy Đo Độ Đáng Yêu" (Cartoon Potion Tubes & Comic Panels)**:
   - Bubbling cartoon Erlenmeyer flasks / thermometer gauges that physically boil over and pop their corks (`BÙM! 9999%!`) when she presses the chunky cartoon lever button.
   - 3 Die-Cut Cartoon Sticker Cards that flip with spring physics (`cubic-bezier(0.34, 1.56, 0.64, 1)`).
4. **Chapter 3 — Chunky Cartoon Blind Box (`POP TOY SERIES`)**:
   - Illustrated 3D toy box with cartoon bunny ears peeking out, wobbling comic physics (`LỌC CỌC!`), a physical perforated zipper strip with an animated SVG scissors icon, and 4 Collectible Chibi Toy Figures + Illustrated Love Coupon Tickets.
5. **Chapter 4 — Whimsical Cartoon Birthday Cake & Living Fire Sprite (Mic Blow-out)**:
   - Hand-drawn multi-tier strawberry-taro cartoon cake with an animated **living cartoon flame character** (with cute eyes and mouth!) that panics and bends when she blows into the Microphone, then puffs into cartoon smoke clouds (`PHÙUU~!`) and reveals a spiral-bound illustrated notebook love letter!
