---
marp: true
theme: uncover
paginate: true
backgroundColor: #0d0d0d
color: #e0e0e0
style: |
  section { font-family: 'Noto Sans JP', 'Helvetica Neue', sans-serif; }
  section.lead h1 { font-size: 64px; color: #fff; }
  section.lead p { color: #888; }
  section.phase { justify-content: center; }
  section.phase h1 { font-size: 120px; color: #1a1a1a; margin-bottom: -20px; font-family: 'Courier New', monospace; }
  section.phase h2 { font-size: 40px; color: #fff; }
  section.phase p { color: #666; }
  h3 { color: #fff; }
  img { border-radius: 12px; border: 1px solid #222; }
  .note { background: #141414; border-left: 3px solid #333; padding: 8px 16px; border-radius: 0 8px 8px 0; font-size: 14px; color: #999; margin-top: 8px; }
  .step-num { display: inline-block; background: #fff; color: #000; width: 32px; height: 32px; text-align: center; line-height: 32px; border-radius: 6px; font-weight: 800; font-size: 14px; margin-right: 8px; }
---

<!-- _class: lead -->

# Google Chat Webhook の追加方法

重要メール通知を Google Chat スペースに
自動送信するための Webhook 設定手順

---

### <span class="step-num">1</span> 「通知用」スペースをクリック

![w:800](https://images.tango.us/workflows/ecff9b15-76cd-440d-9f92-0b102b01785a/steps/48542618-b1fb-442e-b155-d44caf6f66f7/6ed6414a-0603-42bb-b0ba-f6e10bb633d2.png?crop=focalpoint&fit=crop&fp-x=0.4155&fp-y=0.1237&fp-z=2.0536&w=1200)

<div class="note">通知を受け取りたいスペースを開く</div>

---

### <span class="step-num">2</span> 「アプリと統合」をクリック

![w:800](https://images.tango.us/workflows/ecff9b15-76cd-440d-9f92-0b102b01785a/steps/c3e5cf73-f8b5-4bdd-b92a-d958b00ee5cd/818b4e67-45f8-416b-9ca6-86d34afbf914.png?crop=focalpoint&fit=crop&fp-x=0.4472&fp-y=0.4278&fp-z=1.8528&w=1200)

<div class="note">スペースの設定メニューから「アプリと統合」を選択</div>

---

### <span class="step-num">3</span> 「Webhook を追加」をクリック

![w:800](https://images.tango.us/workflows/ecff9b15-76cd-440d-9f92-0b102b01785a/steps/fdb220d1-e3d6-4ebb-a4a2-6e76f81f2e98/8ac895f3-4edd-42ec-84e3-185a6924e9fa.png?crop=focalpoint&fit=crop&fp-x=0.8511&fp-y=0.7912&fp-z=4.0000&w=1200)

---

### <span class="step-num">4</span> 名前に「重要メール通知」と入力

![w:800](https://images.tango.us/workflows/ecff9b15-76cd-440d-9f92-0b102b01785a/steps/a13b28a1-4746-49a1-8714-9cffca805856/4c3d443a-fb7e-4a95-b0a4-807dfb02e5c3.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.4381&fp-z=1.3168&w=1200)

<div class="note">用途がわかる名前を付ける</div>

---

### <span class="step-num">5</span> 「保存」をクリック

![w:800](https://images.tango.us/workflows/ecff9b15-76cd-440d-9f92-0b102b01785a/steps/10d66124-c18b-4635-8f22-417a9ae739e0/80365166-985f-4b92-9152-393e8739b2c8.png?crop=focalpoint&fit=crop&fp-x=0.7361&fp-y=0.6598&fp-z=2.7635&w=1200)

---

### <span class="step-num">6</span> Webhook のオプションメニューを開く

![w:800](https://images.tango.us/workflows/ecff9b15-76cd-440d-9f92-0b102b01785a/steps/36604b31-5866-43a7-a5de-804b7f9c34bc/b4df50c8-e13a-4479-8981-1aa58fbde9b4.png?crop=focalpoint&fit=crop&fp-x=0.9114&fp-y=0.9278&fp-z=4.0000&w=1200)

<div class="note">保存した Webhook の右側にあるメニューアイコンをクリック</div>

---

### <span class="step-num">7</span> 「URL をコピー」をクリック

![w:800](https://images.tango.us/workflows/ecff9b15-76cd-440d-9f92-0b102b01785a/steps/164e7870-bec4-4522-a4fd-777ccdde7bf2/09d03f6e-a6cb-4b8b-a033-31461d000eab.png?crop=focalpoint&fit=crop&fp-x=0.8529&fp-y=0.7990&fp-z=4.0000&w=1200)

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
