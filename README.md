# dog-profile
<p align="center">
  <img src="img/logo.png" width="200" alt="dog-profile logo">
</p>
## 📑 目次
- [プロジェクト概要](#プロジェクト概要)
- [ファイル構成](#ファイル構成)
- [コミットメッセージ命名ルール](#コミットメッセージ命名ルール)
- [運用ルール](#運用ルール)
- [GitHub Pages URL](#github-pages-url)
- [画像サイズの標準](#画像サイズの標準)
- [CSS の命名規則](#css-の命名規則)
- [TODO（今後追加予定）](#todo今後追加予定)

---

## 📌 プロジェクト概要
このリポジトリは、SAKADE の個人サイト **dog-profile** のソースコードを管理するためのものです。  
迷子時の連絡先情報を安全に提示するため、電話番号は画像化して管理し、  
日本語版・ドイツ語版の 2 言語で運用しています。

---

---

## 📝 コミットメッセージ命名ルール

### 1. 基本構造：**動詞 + 対象（現在形）**
例：
- `replace phone number with image`
- `update German phone number`
- `fix contact layout`
- `add AQS-Nummer field`

### 2. 使用する動詞は4種類に統一
#### **add**（追加）
- `add German phone number`
- `add DE contact section`

#### **update**（更新）
- `update JP phone number`
- `update AQS-Nummer`

#### **replace**（置き換え）
- `replace phone number with image`
- `replace contact icons`

#### **fix**（修正）
- `fix contact list spacing`
- `fix typo in German page`

### 3. 対象は具体的に書く
良い例：  
- `update German phone number`  
悪い例：  
- `update stuff`

### 4. 国別・用途別の命名は一貫性を持たせる
- `update JP phone number`  
- `update DE phone number`  
- `update AQS-Nummer`

### 5. 画像変更は **replace** を使う

### 6. 短く・簡潔に・英語で統一

---

## 🔧 運用ルール

### ✔ 電話番号は画像化して管理する
- スクレイピング対策  
- alt 属性には番号を書かない  
- alt はページ言語に合わせる  
  - 日本語：`alt="電話番号"`  
  - ドイツ語：`alt="Telefonnummer"`

### ✔ 国別の番号は JP / DE で分ける
- `/img/phone.png`（日本）  
- `/img/phone_de.png`（ドイツ）

### ✔ AQS-Nummer（検疫番号）は取得後に更新する
コミット例：  
`update AQS-Nummer`

### ✔ GitHub Pages の反映は数十秒かかることがある

---

## 🌐 GitHub Pages URL
https://niwism.github.io/dog-profile/

---

## 🖼 画像サイズの標準
電話番号画像：横 200px 固定
アイコン類：32px × 32px
写真：最大幅 600px（レスポンシブ対応

---

## 🎨 CSS の命名規則
BEM を基本とする（block__element--modifier）
セクション名は英語で統一
色名は役割ベース（primary / accent / warning）
クラス名は小文字・ハイフン区切り

---

## 📌 TODO（今後追加予定）
AQS-Nummer の追加（検疫後）
英語ページ（en.html）の整備
画像の最適化（WebP 化）
GitHub Pages の多言語切り替え改善

------
------
---

# 🇬🇧 English README

## 📌 Project Overview
This repository contains the source code for **dog-profile**, a personal site created by SAKADE.  
To safely display emergency contact information, phone numbers are stored as images.  
The site is available in Japanese, German, and English.

---

## 📁 File Structure
/index.html            # Japanese page
/de.html               # German page
/en.html               # English page
/css/style.css         # Shared styles
/img/phone.png         # Japanese phone number image
/img/phone_de.png      # German phone number image
/README.md             # Project documentation

---

## 📝 Commit Message Naming Rules

### 1. Structure: Verb + Target (present tense)
Examples:
- `replace phone number with image`
- `update German phone number`
- `fix contact layout`
- `add AQS-Nummer field`

### 2. Allowed verbs
- **add**
- **update**
- **replace**
- **fix**

### 3. Be specific  
Good: `update German phone number`  
Bad: `update stuff`

### 4. Use JP / DE / AQS for clarity  
- `update JP phone number`  
- `update DE phone number`  
- `update AQS-Nummer`

### 5. Use replace for image changes  
### 6. Keep messages short and simple

---

## 🔧 Operational Rules

### ✔ Phone numbers must be stored as images
- Prevent scraping  
- alt text must not contain the number  
- alt text should match the page language

### ✔ Separate JP / DE phone numbers  
### ✔ Update AQS-Nummer after quarantine  
### ✔ GitHub Pages may take several seconds to update

---

## 🌐 GitHub Pages URL (EN)
https://niwism.github.io/dog-profile/

---

## 🖼 Image Size Standards
Phone number images: 200px width
Icons: 32px × 32px
Photos: max width 600px (responsive)

---

## 🎨 CSS Naming ConvUse BEM (block__element--modifier)
Section names in English
Role-based color names (primary / accent / warning)
Lowercase, hyphen-separated class namesentions

---

## 📌 TODO
Add AQS-Nummer after quarantine
Improve English page (en.html)
Convert images to WebP
Enhance multilingual switching for GitHub Pages

