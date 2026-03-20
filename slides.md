---
marp: true
theme: default
paginate: true
backgroundColor: #ffffff
color: #333333
style: |
  section { font-family: 'Noto Sans JP', 'Helvetica Neue', sans-serif; }
  section.lead { background: #f8f9fa; }
  section.lead h1 { font-size: 64px; color: #1a73e8; }
  section.lead p { color: #666; }
  h3 { color: #333; }
  strong { color: #1a73e8; }
  img { border-radius: 12px; border: 1px solid #e0e0e0; }
  .note { background: #f0f4ff; border-left: 3px solid #1a73e8; padding: 8px 16px; border-radius: 0 8px 8px 0; font-size: 14px; color: #555; margin-top: 8px; }
  .step-num { display: inline-block; background: #1a73e8; color: #fff; width: 32px; height: 32px; text-align: center; line-height: 32px; border-radius: 6px; font-weight: 800; font-size: 14px; margin-right: 8px; }
---

<!-- _class: lead -->

# Google Chat Webhook の追加方法

重要メール通知を Google Chat スペースに
自動送信するための Webhook 設定手順

---

### <span class="step-num">1</span> 「通知用」スペースをクリック

![w:800](images/step-2.png)

<div class="note">通知を受け取りたいスペースを開く</div>

---

### <span class="step-num">2</span> 「アプリと統合」をクリック

![w:800](images/step-3.png)

<div class="note">スペースの設定メニューから「アプリと統合」を選択</div>

---

### <span class="step-num">3</span> 「Webhook を追加」をクリック

![w:800](images/step-4.png)

---

### <span class="step-num">4</span> 名前に「重要メール通知」と入力

![w:800](images/step-5.png)

<div class="note">用途がわかる名前を付ける</div>

---

### <span class="step-num">5</span> 「保存」をクリック

![w:800](images/step-6.png)

---

### <span class="step-num">6</span> Webhook のオプションメニューを開く

![w:800](images/step-7a.png)

<div class="note">保存した Webhook の右側にあるメニューアイコンをクリック</div>

---

### <span class="step-num">7</span> 「URL をコピー」をクリック

![w:800](images/step-7b.png)

<div class="note">コピーした URL を GAS やスクリプトに貼り付けて使用</div>

---

### 活用のコツ

- **1スペース1用途** — 通知の種類ごとにスペースを分けると見やすい
- **Webhook URL は秘密情報** — 知っている人は誰でも投稿できるので漏洩注意
- **GAS と組み合わせ** — Gmail の重要メールを自動で Chat に転送できる

---

<!-- _class: lead -->

# これで Webhook 設定完了

コピーした URL を GAS や自動化ツールに
貼り付けて通知を飛ばしましょう
