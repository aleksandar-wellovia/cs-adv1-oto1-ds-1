# Content Style Template Reference

All main CSS classes are preserved in `index.html` `<style>` block.
This file documents the HTML patterns and their styles for re-use.

## Container Structure
```html
<div class="content-edit-anchor warming-oil-content warming-oil-source">
  <section>
    ...content...
  </section>
</div>
```
- Sections: `border-bottom: 1px solid #EADFD2`, padding/margin ~30px
- Max width: 900px, centered

## Section Heading (h2)
```html
<h2>Section Title Here</h2>
```
- Poppins 700, 35px/1.2, color #17222E, center-aligned
- Mobile: 30px

## Body Paragraph (.line)
```html
<p class="line">Regular paragraph text.</p>
<p class="line b">Bold emphasis paragraph.</p>
```
- Poppins 400, 17px/1.55, color #23201c
- `.b` = font-weight 700
- margin: 0 0 13px

## Red Highlight
```html
<span class="red">red text</span>
```
- color: #e91111

## Big Idea (.bigidea)
```html
<p class="bigidea">Centered sub-heading text</p>
```
- Poppins 700, 24px/1.3, color rgb(5,47,85), center
- Mobile: 22px

## Stat Heading
```html
<h2 class="stat-heading">Big stat<br><u>Underlined part</u></h2>
```
- 30px/1.25, center (mobile: 24px)
- Inline CSS (saved below)

## Image (.photo + .content-photo)
```html
<div class="photo content-photo"><img src="file.png" alt="desc"></div>
```
- Max-width 900px, centered, border-radius 10px (mobile 8px)
- Hero variant: `.photo1-hero` (same but 900px full-width)
- Guarantee: `.guarantee-photo` (full-width 900px)
- Scarcity: `.scarcity-product-visual` (with price badge overlay)

## Video (.content-video)
```html
<div class="photo content-video"><video src="file.mp4" autoplay muted loop playsinline preload="metadata"></video></div>
```

## Green Highlight Box (.greenbox)
```html
<div class="greenbox">
  <p class="gline"><b>Bold header</b></p>
  <p class="gline">&#9989; Benefit point</p>
  <p class="gline">&#10060; Negative point</p>
</div>
```
- bg #FAF4EE, border 1.5px solid #EADFD2, radius 14px, padding 18px 20px
- `.gline` = same as `.line` (17px/1.55)

## Cross Box (.xbox)
```html
<div class="xbox">
  <p class="xline"><b>Step title</b><br>Description.</p>
  <p class="xline">Another item.</p>
</div>
```
- bg #FAF4EE, border 1px solid #EADFD2, radius 14px, padding 16px 18px 4px
- `.xline` = same as `.line` (17px/1.55)

## Review Card (INLINE CSS - removed from page, saved here)
```css
.review-card{width:70%;margin:0 auto 22px;padding:12px 10px 16px;background-color:#faf4ee;border:1.5px solid #EADFD2;box-shadow:5px 5px 5px 0 rgba(155,155,155,1);border-radius:14px;text-align:center;display:flex;flex-direction:column;align-items:center;}
.rev-photo{height:200px;width:200px;object-fit:cover;border-radius:100px;margin-top:10px;box-shadow:5px 5px 5px 0 rgba(155,155,155,1);border:6px double #042F55;}
.rev-name{font-family:Poppins,Arial,sans-serif;font-size:17px;line-height:1.3;font-weight:700;text-align:center;margin:10px 0 5px;padding:10px 10px 5px;}
.rev-stars{font-family:Poppins,Arial,sans-serif;font-size:17px;line-height:1.3;font-weight:700;text-align:center;margin:5px 0;padding:1px 10px;}
.rev-verified{font-family:Poppins,Arial,sans-serif;font-size:17px;line-height:1.3;font-weight:700;text-align:center;color:#417505;margin:1px 0 5px;padding:1px 10px;}
.rev-quote{font-family:Poppins,Arial,sans-serif;font-size:17px;line-height:1.55;font-weight:400;text-align:center;margin-top:5px;padding:10px;}
.stat-heading{font-size:30px;line-height:1.25;text-align:center;margin:26px 0 18px;}
@media (max-width:600px){.review-card{width:92%;}.stat-heading{font-size:24px;}}
```
```html
<div class="review-card">
  <img class="rev-photo" src="photo.webp" alt="Name, Location">
  <p class="rev-name">Janet R., Tennessee</p>
  <p class="rev-stars">&#11088;&#11088;&#11088;&#11088;&#11088;</p>
  <p class="rev-verified">Verified Review</p>
  <p class="rev-quote">"Review quote text."</p>
</div>
```

## Guarantee Badge (INLINE CSS - removed from page, saved here)
```css
.warming-oil-source .guarantee-badge img{max-width:240px !important;width:60% !important;height:auto !important;margin:4px auto 2px !important;display:block !important;box-shadow:none !important;border:none !important;}
.warming-oil-source .guarantee-badge{margin:4px 0 10px !important;}
```

## Section Separator
```html
<hr class="headline-break">
```
- 1px solid #e2e2e2, max-width 900px, centered

## Decline Link
```html
<div class="decline"><i>No thank you. Decline text here.</i></div>
```
- color #53595F, 15px, underline, cursor pointer

## CTA Button
```html
<div class="addbtn"><span class="addbtn-main">YES! Button Text</span><span class="addbtn-sub">Sub-text line</span></div>
```
- bg rgb(4,47,85), white text, rounded 60px, shadow, 19px/800
- Sub: 13px/600
