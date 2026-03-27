---
marp: true
theme: default
paginate: true
header: ''
footer: ''
style: |
  section {
    font-family: 'Hiragino Sans', 'Noto Sans JP', sans-serif;
    background-color: #ffffff;
    padding: 50px 60px;
  }
  header { display: none; }
  h1 { font-size: 44px; color: #1f2937; font-weight: 800; margin-bottom: 16px; line-height: 1.3; }
  h2 { font-size: 32px; color: #374151; font-weight: 700; margin-bottom: 16px; }
  h3 { font-size: 26px; color: #4b5563; font-weight: 600; margin-bottom: 12px; }
  p, li { font-size: 22px; line-height: 1.7; color: #374151; }
  ul, ol { margin-left: 24px; }
  li { margin-bottom: 8px; }
  strong { color: #1f2937; font-weight: 700; }
  blockquote { border-left: 4px solid #028090; padding-left: 16px; margin: 16px 0; color: #4b5563; font-size: 22px; }
---

<script src="../theme/js/tailwindcss-3.0.16.js"></script>
<script src="../theme/js/tailwind.config.js"></script>

<!-- _class: lead -->
<!-- _paginate: false -->
<!--
_backgroundImage: "linear-gradient(135deg, #028090 0%, #00A896 50%, #02C39A 100%)"
_color: #fff
-->

<div style="text-align: center;">

# アプリ開発のハードルが変わった

<p style="font-size: 28px; opacity: 0.9; margin-top: 24px;">バイブコーディング体験ワークショップ</p>

<p style="font-size: 20px; opacity: 0.7; margin-top: 40px;">2026年4月2日 ｜ ZOUさん社内研修</p>

</div>

---

# こんなこと思ったことありませんか

<div style="display: flex; flex-direction: column; gap: 14px; margin-top: 20px;">
  <div style="background: #f9fafb; border-radius: 12px; padding: 18px 24px; border-left: 4px solid #d1d5db;">
    <p style="font-size: 21px; color: #374151;">「営業の日報、もっとラクに入力できないかな」</p>
  </div>
  <div style="background: #f9fafb; border-radius: 12px; padding: 18px 24px; border-left: 4px solid #d1d5db;">
    <p style="font-size: 21px; color: #374151;">「撮影素材の管理、フォルダが増えすぎて探すのが大変」</p>
  </div>
  <div style="background: #f9fafb; border-radius: 12px; padding: 18px 24px; border-left: 4px solid #d1d5db;">
    <p style="font-size: 21px; color: #374151;">「クライアントからの修正依頼、どれが最新か分からなくなる」</p>
  </div>
</div>

<div style="background: #f0fdf9; border-radius: 12px; padding: 18px 24px; margin-top: 24px; text-align: center;">
  <p style="font-size: 22px; color: #028090; font-weight: 700;">でも、便利なツールを作るのはエンジニアの仕事だし...</p>
  <p style="font-size: 20px; color: #6b7280; margin-top: 4px;">外注すると高いし、時間もかかるし、ちょっとしたことでは頼めない</p>
</div>

---

# その常識が変わりました

<!-- _paginate: false -->

<p style="font-size: 20px; color: #6b7280; margin-bottom: 12px;">今は、こんな時代になっています</p>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 340" font-family="'Hiragino Sans', 'Noto Sans JP', sans-serif" style="width: 100%; max-height: 420px;">
  <rect x="20" y="20" width="360" height="300" rx="16" fill="#f9fafb" stroke="#e5e7eb" stroke-width="2"/>
  <text x="200" y="56" text-anchor="middle" font-size="18" font-weight="700" fill="#991b1b">従来の開発</text>
  <rect x="50" y="76" width="300" height="44" rx="8" fill="#fef2f2"/>
  <text x="200" y="104" text-anchor="middle" font-size="15" fill="#374151">要件をまとめる（数週間）</text>
  <line x1="200" y1="120" x2="200" y2="130" stroke="#d1d5db" stroke-width="2"/>
  <polygon points="200,136 194,126 206,126" fill="#d1d5db"/>
  <rect x="50" y="136" width="300" height="44" rx="8" fill="#fef2f2"/>
  <text x="200" y="164" text-anchor="middle" font-size="15" fill="#374151">エンジニアに依頼（数十万〜）</text>
  <line x1="200" y1="180" x2="200" y2="190" stroke="#d1d5db" stroke-width="2"/>
  <polygon points="200,196 194,186 206,186" fill="#d1d5db"/>
  <rect x="50" y="196" width="300" height="44" rx="8" fill="#fef2f2"/>
  <text x="200" y="224" text-anchor="middle" font-size="15" fill="#374151">開発を待つ（数ヶ月）</text>
  <line x1="200" y1="240" x2="200" y2="250" stroke="#d1d5db" stroke-width="2"/>
  <polygon points="200,256 194,246 206,246" fill="#d1d5db"/>
  <rect x="50" y="256" width="300" height="44" rx="8" fill="#fef2f2"/>
  <text x="200" y="284" text-anchor="middle" font-size="15" fill="#374151">やっと完成</text>
  <rect x="420" y="20" width="360" height="300" rx="16" fill="#f0fdf9" stroke="#028090" stroke-width="2"/>
  <text x="600" y="56" text-anchor="middle" font-size="18" font-weight="700" fill="#028090">バイブコーディング</text>
  <rect x="450" y="76" width="300" height="44" rx="8" fill="white" stroke="#028090" stroke-width="1.5"/>
  <text x="600" y="104" text-anchor="middle" font-size="15" fill="#374151" font-weight="600">困りごとを言葉にする</text>
  <line x1="600" y1="120" x2="600" y2="130" stroke="#028090" stroke-width="2"/>
  <polygon points="600,136 594,126 606,126" fill="#028090"/>
  <rect x="450" y="136" width="300" height="44" rx="8" fill="white" stroke="#00A896" stroke-width="1.5"/>
  <text x="600" y="164" text-anchor="middle" font-size="15" fill="#374151" font-weight="600">AIに「作って」と伝える</text>
  <line x1="600" y1="180" x2="600" y2="190" stroke="#00A896" stroke-width="2"/>
  <polygon points="600,196 594,186 606,186" fill="#00A896"/>
  <rect x="450" y="196" width="300" height="44" rx="8" fill="white" stroke="#02C39A" stroke-width="1.5"/>
  <text x="600" y="224" text-anchor="middle" font-size="15" fill="#374151" font-weight="600">数分で動くものが完成</text>
  <line x1="600" y1="240" x2="600" y2="250" stroke="#02C39A" stroke-width="2"/>
  <polygon points="600,256 594,246 606,246" fill="#02C39A"/>
  <rect x="450" y="256" width="300" height="44" rx="8" fill="#028090"/>
  <text x="600" y="284" text-anchor="middle" font-size="15" fill="white" font-weight="700">「直して」で改善を繰り返す</text>
  <text x="400" y="180" text-anchor="middle" font-size="28" fill="#028090">→</text>
</svg>

---

# 身近なことに例えると

<p style="font-size: 20px; color: #6b7280; margin-bottom: 20px;">バイブコーディングは、実は皆さんが毎日やっていることと同じです</p>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
  <div style="background: #f9fafb; border-radius: 16px; padding: 24px;">
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 10px;">レストランで注文するとき</p>
    <p style="font-size: 20px; color: #374151; line-height: 1.7;">料理の作り方を知らなくても<br>「辛さ控えめのパスタ」と伝えれば<br>シェフが作ってくれる</p>
  </div>
  <div style="background: #f9fafb; border-radius: 16px; padding: 24px;">
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 10px;">美容室でオーダーするとき</p>
    <p style="font-size: 20px; color: #374151; line-height: 1.7;">カットの技術がなくても<br>「こんな感じにしたい」と伝えれば<br>美容師さんが仕上げてくれる</p>
  </div>
</div>

<div style="background: #f0fdf9; border: 2px solid #028090; border-radius: 16px; padding: 24px; margin-top: 20px; text-align: center;">
  <p style="font-size: 24px; font-weight: 700; color: #028090;">バイブコーディングも同じ</p>
  <p style="font-size: 20px; margin-top: 6px; color: #374151;">「こんなツールが欲しい」と伝えれば、AIが作ってくれる</p>
</div>

---

# バイブコーディングとは

<div style="background: #f0fdf9; border-radius: 16px; padding: 28px 32px; margin-top: 12px; border-left: 6px solid #028090;">
  <p style="font-size: 26px; color: #1f2937; line-height: 1.6;">AIに<strong style="color: #028090;">「こんなものを作りたい」</strong>と日本語で伝えながら、<br>会話のやりとりでツールを作っていく方法</p>
</div>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 24px;">
  <div style="background: #f9fafb; border-radius: 12px; padding: 20px;">
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 8px;">必要なスキル</p>
    <p style="font-size: 20px; color: #1f2937; font-weight: 600;">「困っていること」を言葉にする力</p>
    <p style="font-size: 17px; color: #6b7280; margin-top: 4px;">普段の仕事で誰もがやっていること</p>
  </div>
  <div style="background: #f9fafb; border-radius: 12px; padding: 20px;">
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 8px;">不要なスキル</p>
    <p style="font-size: 20px; color: #1f2937; font-weight: 600;">プログラミング・英語・IT知識</p>
    <p style="font-size: 17px; color: #6b7280; margin-top: 4px;">全部AIがやってくれる</p>
  </div>
</div>

<div style="background: #f9fafb; border-radius: 12px; padding: 14px 20px; margin-top: 20px; text-align: center;">
  <p style="font-size: 19px; color: #6b7280;"><strong style="color: #028090;">バイブ</strong> = 雰囲気、ノリ。細かいことは気にせず「ノリと勢いでAIに作ってもらう」スタイル</p>
  <p style="font-size: 17px; color: #9ca3af; margin-top: 4px;">2025年2月、ChatGPTを作った会社のトップが提唱して話題に</p>
</div>

---

# バイブコーディングの全体像

<p style="font-size: 20px; color: #6b7280; margin-bottom: 8px;">4つのステップで、アイデアが動くツールになる</p>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 280" font-family="'Hiragino Sans', 'Noto Sans JP', sans-serif" style="width: 100%; max-height: 360px;">
  <rect x="10" y="40" width="160" height="180" rx="14" fill="#f9fafb" stroke="#028090" stroke-width="2"/>
  <circle cx="90" cy="76" r="22" fill="#028090"/>
  <text x="90" y="83" text-anchor="middle" font-size="20" font-weight="800" fill="white">1</text>
  <text x="90" y="116" text-anchor="middle" font-size="16" font-weight="700" fill="#1f2937">困りごとを</text>
  <text x="90" y="138" text-anchor="middle" font-size="16" font-weight="700" fill="#1f2937">言葉にする</text>
  <text x="90" y="172" text-anchor="middle" font-size="13" fill="#6b7280">「日報入力が</text>
  <text x="90" y="190" text-anchor="middle" font-size="13" fill="#6b7280">大変...」</text>
  <line x1="176" y1="130" x2="200" y2="130" stroke="#028090" stroke-width="2.5"/>
  <polygon points="206,130 196,124 196,136" fill="#028090"/>
  <rect x="212" y="40" width="160" height="180" rx="14" fill="#f9fafb" stroke="#00A896" stroke-width="2"/>
  <circle cx="292" cy="76" r="22" fill="#00A896"/>
  <text x="292" y="83" text-anchor="middle" font-size="20" font-weight="800" fill="white">2</text>
  <text x="292" y="116" text-anchor="middle" font-size="16" font-weight="700" fill="#1f2937">AIに</text>
  <text x="292" y="138" text-anchor="middle" font-size="16" font-weight="700" fill="#1f2937">伝える</text>
  <text x="292" y="172" text-anchor="middle" font-size="13" fill="#6b7280">「こんなツール</text>
  <text x="292" y="190" text-anchor="middle" font-size="13" fill="#6b7280">作りたい」</text>
  <line x1="378" y1="130" x2="402" y2="130" stroke="#00A896" stroke-width="2.5"/>
  <polygon points="408,130 398,124 398,136" fill="#00A896"/>
  <rect x="414" y="40" width="160" height="180" rx="14" fill="#f9fafb" stroke="#02C39A" stroke-width="2"/>
  <circle cx="494" cy="76" r="22" fill="#02C39A"/>
  <text x="494" y="83" text-anchor="middle" font-size="20" font-weight="800" fill="white">3</text>
  <text x="494" y="116" text-anchor="middle" font-size="16" font-weight="700" fill="#1f2937">AIが</text>
  <text x="494" y="138" text-anchor="middle" font-size="16" font-weight="700" fill="#1f2937">作ってくれる</text>
  <text x="494" y="172" text-anchor="middle" font-size="13" fill="#6b7280">数分で最初の</text>
  <text x="494" y="190" text-anchor="middle" font-size="13" fill="#6b7280">バージョン完成</text>
  <line x1="580" y1="130" x2="604" y2="130" stroke="#02C39A" stroke-width="2.5"/>
  <polygon points="610,130 600,124 600,136" fill="#02C39A"/>
  <rect x="616" y="40" width="170" height="180" rx="14" fill="#028090"/>
  <circle cx="701" cy="76" r="22" fill="white"/>
  <text x="701" y="83" text-anchor="middle" font-size="20" font-weight="800" fill="#028090">4</text>
  <text x="701" y="116" text-anchor="middle" font-size="16" font-weight="700" fill="white">直してもらう</text>
  <text x="701" y="138" text-anchor="middle" font-size="16" font-weight="700" fill="white">を繰り返す</text>
  <text x="701" y="172" text-anchor="middle" font-size="13" fill="rgba(255,255,255,0.8)">「ここ変えて」</text>
  <text x="701" y="190" text-anchor="middle" font-size="13" fill="rgba(255,255,255,0.8)">で改善</text>
  <path d="M 701 226 L 701 254 Q 701 264 691 264 L 504 264 Q 494 264 494 254 L 494 232" fill="none" stroke="#028090" stroke-width="2" stroke-dasharray="6,4"/>
  <polygon points="494,226 488,236 500,236" fill="#028090"/>
  <text x="598" y="260" text-anchor="middle" font-size="12" fill="#028090" font-weight="600">繰り返し改善</text>
</svg>

<div style="background: #f0fdf9; border-radius: 12px; padding: 14px 20px; margin-top: 12px; text-align: center;">
  <p style="font-size: 19px; color: #028090; font-weight: 600;">美容室で「もう少し短く」「前髪はこのくらい」と伝えながら仕上げるのと同じ感覚</p>
</div>

---

# 実際に作った事例 営業報告ツール

<p style="font-size: 20px; color: #6b7280; margin-bottom: 12px;">バイブコーディングで実際に作ったツールがこちら</p>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
  <div>
    <p style="font-size: 16px; color: #991b1b; font-weight: 700; letter-spacing: 1px; margin-bottom: 12px;">営業チームの困りごと</p>
    <div style="display: flex; flex-direction: column; gap: 8px;">
      <div style="background: #fef2f2; border-radius: 10px; padding: 14px 18px;">
        <p style="font-size: 18px; color: #374151;">訪問後にオフィスに戻ってから日報入力</p>
      </div>
      <div style="background: #fef2f2; border-radius: 10px; padding: 14px 18px;">
        <p style="font-size: 18px; color: #374151;">1日に何件も回ると内容を忘れる</p>
      </div>
      <div style="background: #fef2f2; border-radius: 10px; padding: 14px 18px;">
        <p style="font-size: 18px; color: #374151;">移動中はキーボード入力が難しい</p>
      </div>
    </div>
  </div>
  <div style="background: #f0fdf9; border: 2px solid #028090; border-radius: 16px; padding: 24px;">
    <p style="font-size: 16px; font-weight: 700; letter-spacing: 1px; margin-bottom: 12px; color: #028090;">作ったもの</p>
    <div style="display: flex; flex-direction: column; gap: 10px;">
      <div style="background: white; border-radius: 10px; padding: 12px 16px;">
        <p style="font-size: 18px; font-weight: 600; color: #374151;">音声で話すだけで日報が書ける</p>
      </div>
      <div style="background: white; border-radius: 10px; padding: 12px 16px;">
        <p style="font-size: 18px; font-weight: 600; color: #374151;">AIが「次回アクションは」と質問してくれる</p>
      </div>
      <div style="background: white; border-radius: 10px; padding: 12px 16px;">
        <p style="font-size: 18px; font-weight: 600; color: #374151;">スマホのブラウザだけで完結する</p>
      </div>
    </div>
  </div>
</div>

<div style="background: #f9fafb; border-radius: 12px; padding: 16px 20px; margin-top: 16px; text-align: center;">
  <p style="font-size: 20px; color: #1f2937; font-weight: 700;">この後、矢野さんから実際の画面をお見せします</p>
</div>

---

# Step 1 困りごとを言葉にする

<p style="font-size: 20px; color: #6b7280; margin-bottom: 16px;">最初のステップは「何に困っているか」を整理すること。完璧じゃなくてOK</p>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
  <div>
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 12px;">こんなふうに思ったら、それが出発点</p>
    <div style="display: flex; flex-direction: column; gap: 10px;">
      <div style="background: #f9fafb; border-radius: 10px; padding: 14px 18px;">
        <p style="font-size: 18px; color: #374151;">「撮影スケジュール、Excelだと共有しにくい」</p>
      </div>
      <div style="background: #f9fafb; border-radius: 10px; padding: 14px 18px;">
        <p style="font-size: 18px; color: #374151;">「クライアントへの見積もり、毎回似た作業」</p>
      </div>
      <div style="background: #f9fafb; border-radius: 10px; padding: 14px 18px;">
        <p style="font-size: 18px; color: #374151;">「案件ごとの進捗が一目で分かるといいのに」</p>
      </div>
      <div style="background: #f9fafb; border-radius: 10px; padding: 14px 18px;">
        <p style="font-size: 18px; color: #374151;">「納品データの受け渡し、もっとスムーズにしたい」</p>
      </div>
    </div>
  </div>
  <div style="background: #f0fdf9; border: 2px solid #028090; border-radius: 16px; padding: 24px; display: flex; flex-direction: column; justify-content: center;">
    <p style="font-size: 22px; font-weight: 700; margin-bottom: 12px; color: #028090;">コツ</p>
    <p style="font-size: 18px; line-height: 1.8; color: #374151;">漠然とした不満でOK。<br>「なんとなく不便」でも大丈夫。<br><br>AIに話しているうちに<br>「本当に必要なもの」が<br>見えてきます。</p>
  </div>
</div>

---

# Step 2 AIに「こんなの作って」と伝える

<p style="font-size: 20px; color: #6b7280; margin-bottom: 12px;">困りごとが見えたら、AIにそのまま伝える。堅い言葉でなくて大丈夫</p>

<div style="background: #f9fafb; border-radius: 16px; padding: 24px 28px;">
  <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 16px;">会話のイメージ</p>
  <div style="display: flex; flex-direction: column; gap: 10px;">
    <div style="display: flex; align-items: center; gap: 12px;">
      <span style="background: #e5e7eb; border-radius: 8px; padding: 4px 10px; font-size: 13px; font-weight: 700; color: #6b7280; white-space: nowrap;">あなた</span>
      <div style="background: white; border-radius: 12px; padding: 12px 16px; box-shadow: 0 1px 3px rgba(0,0,0,0.08); flex: 1;">
        <p style="font-size: 18px; color: #374151;">営業で客先を回った後の日報入力が大変。もっとラクにしたい</p>
      </div>
    </div>
    <div style="display: flex; align-items: center; gap: 12px;">
      <span style="background: #028090; border-radius: 8px; padding: 4px 10px; font-size: 13px; font-weight: 700; color: white; white-space: nowrap;">AI</span>
      <div style="background: #f0fdf9; border-radius: 12px; padding: 12px 16px; flex: 1;">
        <p style="font-size: 18px; color: #374151;">日報にはどんな項目がありますか。訪問先名、内容、次のアクションなど</p>
      </div>
    </div>
    <div style="display: flex; align-items: center; gap: 12px;">
      <span style="background: #e5e7eb; border-radius: 8px; padding: 4px 10px; font-size: 13px; font-weight: 700; color: #6b7280; white-space: nowrap;">あなた</span>
      <div style="background: white; border-radius: 12px; padding: 12px 16px; box-shadow: 0 1px 3px rgba(0,0,0,0.08); flex: 1;">
        <p style="font-size: 18px; color: #374151;">訪問先と日時と、話した内容のメモ。あと次にやることも書きたい</p>
      </div>
    </div>
    <div style="display: flex; align-items: center; gap: 12px;">
      <span style="background: #028090; border-radius: 8px; padding: 4px 10px; font-size: 13px; font-weight: 700; color: white; white-space: nowrap;">AI</span>
      <div style="background: #f0fdf9; border-radius: 12px; padding: 12px 16px; flex: 1;">
        <p style="font-size: 18px; color: #374151;">わかりました。スマホから使えるシンプルな日報ツールを作りますね</p>
      </div>
    </div>
  </div>
</div>

---

# Step 3 AIが作ってくれる → 確認する

<p style="font-size: 20px; color: #6b7280; margin-bottom: 16px;">AIに伝えると、数分でブラウザで動くツールが出来上がる</p>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
  <div>
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 12px;">出来上がりのイメージ</p>
    <div style="background: #f9fafb; border: 2px solid #e5e7eb; border-radius: 12px; padding: 16px 20px;">
      <div style="background: #028090; border-radius: 8px 8px 0 0; padding: 8px 12px; margin: -16px -20px 12px -20px;">
        <p style="font-size: 14px; color: white; font-weight: 600;">営業日報ツール</p>
      </div>
      <div style="background: #e5e7eb; border-radius: 6px; padding: 8px 12px; margin-bottom: 8px;">
        <p style="font-size: 14px; color: #9ca3af;">訪問先を入力...</p>
      </div>
      <div style="background: #e5e7eb; border-radius: 6px; padding: 8px 12px; margin-bottom: 8px;">
        <p style="font-size: 14px; color: #9ca3af;">日時を選択...</p>
      </div>
      <div style="background: #e5e7eb; border-radius: 6px; padding: 8px 12px; height: 48px; margin-bottom: 12px;">
        <p style="font-size: 14px; color: #9ca3af;">商談メモ...</p>
      </div>
      <div style="background: #028090; border-radius: 6px; padding: 8px; text-align: center;">
        <p style="font-size: 14px; color: white; font-weight: 600;">保存する</p>
      </div>
    </div>
    <p style="font-size: 16px; color: #6b7280; margin-top: 8px; text-align: center;">スマホやPCのブラウザで<br>そのまま使える</p>
  </div>
  <div style="display: flex; flex-direction: column; justify-content: center;">
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 12px;">あなたがやること</p>
    <div style="display: flex; flex-direction: column; gap: 12px;">
      <div style="background: #f9fafb; border-radius: 10px; padding: 16px;">
        <p style="font-size: 20px; color: #1f2937; font-weight: 600;">出来上がった画面を触ってみる</p>
      </div>
      <div style="background: #f9fafb; border-radius: 10px; padding: 16px;">
        <p style="font-size: 20px; color: #1f2937; font-weight: 600;">「ここが違うな」を見つける</p>
      </div>
      <div style="background: #f9fafb; border-radius: 10px; padding: 16px;">
        <p style="font-size: 20px; color: #1f2937; font-weight: 600;">AIに「ここ直して」と伝える</p>
      </div>
    </div>
  </div>
</div>

---

# Step 4 「直して」を繰り返して完成させる

<p style="font-size: 20px; color: #6b7280; margin-bottom: 8px;">一発で完璧にはならない。でも「直して」と言えば何度でも直してくれる</p>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: center;">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 480 340" font-family="'Hiragino Sans', 'Noto Sans JP', sans-serif" style="width: 100%; max-height: 380px;">
    <rect x="150" y="16" width="180" height="56" rx="28" fill="#028090"/>
    <text x="240" y="50" text-anchor="middle" font-size="16" font-weight="700" fill="white">触ってみる</text>
    <path d="M 336 44 Q 390 44 390 94" fill="none" stroke="#028090" stroke-width="2.5"/>
    <polygon points="390,100 384,90 396,90" fill="#028090"/>
    <rect x="310" y="106" width="160" height="56" rx="28" fill="#00A896"/>
    <text x="390" y="140" text-anchor="middle" font-size="15" font-weight="700" fill="white">「ここが違うな」</text>
    <path d="M 390 168 Q 390 220 336 220" fill="none" stroke="#00A896" stroke-width="2.5"/>
    <polygon points="330,220 340,214 340,226" fill="#00A896"/>
    <rect x="150" y="192" width="180" height="56" rx="28" fill="#02C39A"/>
    <text x="240" y="226" text-anchor="middle" font-size="16" font-weight="700" fill="white">AIに「直して」</text>
    <path d="M 144 220 Q 90 220 90 174" fill="none" stroke="#02C39A" stroke-width="2.5"/>
    <polygon points="90,168 84,178 96,178" fill="#02C39A"/>
    <rect x="10" y="106" width="160" height="56" rx="28" fill="#028090"/>
    <text x="90" y="140" text-anchor="middle" font-size="16" font-weight="700" fill="white">AIが修正する</text>
    <path d="M 90 100 Q 90 44 138 44" fill="none" stroke="#028090" stroke-width="2.5"/>
    <polygon points="144,44 134,38 134,50" fill="#028090"/>
    <text x="240" y="130" text-anchor="middle" font-size="14" font-weight="700" fill="#028090">何度でも</text>
    <text x="240" y="148" text-anchor="middle" font-size="14" font-weight="700" fill="#028090">繰り返せる</text>
    <rect x="80" y="280" width="320" height="44" rx="10" fill="#f0fdf9" stroke="#028090" stroke-width="1.5"/>
    <text x="240" y="308" text-anchor="middle" font-size="14" fill="#028090" font-weight="600">遠慮なく何度でもOK。AIは嫌な顔をしません</text>
  </svg>
  <div>
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 12px;">こんなふうに伝えるだけ</p>
    <div style="display: flex; flex-direction: column; gap: 10px;">
      <div style="background: #f9fafb; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #028090;">
        <p style="font-size: 17px; color: #374151;">「文字が小さくて読みにくい」</p>
      </div>
      <div style="background: #f9fafb; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #00A896;">
        <p style="font-size: 17px; color: #374151;">「前回の候補が出ると便利」</p>
      </div>
      <div style="background: #f9fafb; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #02C39A;">
        <p style="font-size: 17px; color: #374151;">「撮影日だけ色付きにして」</p>
      </div>
    </div>
  </div>
</div>

---

# できること・できないこと

<p style="font-size: 20px; color: #6b7280; margin-bottom: 16px;">万能ではないので、得意なことと苦手なことを知っておくと安心</p>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
  <div style="border-radius: 16px; padding: 24px; border: 2px solid #d1fae5;">
    <p style="font-size: 16px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 14px;">得意なこと</p>
    <div style="display: flex; flex-direction: column; gap: 10px;">
      <div style="background: #f0fdf9; border-radius: 8px; padding: 10px 14px;">
        <p style="font-size: 18px; color: #374151;">シンプルな業務ツール</p>
        <p style="font-size: 15px; color: #6b7280;">日報入力、TODO管理、スケジュール共有</p>
      </div>
      <div style="background: #f0fdf9; border-radius: 8px; padding: 10px 14px;">
        <p style="font-size: 18px; color: #374151;">データの入力・表示・集計</p>
        <p style="font-size: 15px; color: #6b7280;">撮影案件の一覧管理、顧客情報の検索</p>
      </div>
      <div style="background: #f0fdf9; border-radius: 8px; padding: 10px 14px;">
        <p style="font-size: 18px; color: #374151;">繰り返し作業の効率化</p>
        <p style="font-size: 15px; color: #6b7280;">見積もりテンプレ、撮影スケジュール表など</p>
      </div>
    </div>
  </div>
  <div style="border-radius: 16px; padding: 24px; border: 2px solid #fecaca;">
    <p style="font-size: 16px; color: #991b1b; font-weight: 700; letter-spacing: 1px; margin-bottom: 14px;">苦手なこと</p>
    <div style="display: flex; flex-direction: column; gap: 10px;">
      <div style="background: #fef2f2; border-radius: 8px; padding: 10px 14px;">
        <p style="font-size: 18px; color: #374151;">大人数が同時に使うシステム</p>
        <p style="font-size: 15px; color: #6b7280;">数百人が使う受注管理システムなど</p>
      </div>
      <div style="background: #fef2f2; border-radius: 8px; padding: 10px 14px;">
        <p style="font-size: 18px; color: #374151;">お金や個人情報を扱うもの</p>
        <p style="font-size: 15px; color: #6b7280;">クレジットカード決済、顧客データの一括管理</p>
      </div>
      <div style="background: #fef2f2; border-radius: 8px; padding: 10px 14px;">
        <p style="font-size: 18px; color: #374151;">既存の社内システムとの連携</p>
        <p style="font-size: 15px; color: #6b7280;">会計ソフトや勤怠管理との自動連携</p>
      </div>
    </div>
  </div>
</div>

---

# 使い方のコツ

<p style="font-size: 20px; color: #6b7280; margin-bottom: 16px;">AIとうまく会話するための3つのポイント</p>

<div style="display: flex; flex-direction: column; gap: 14px;">
  <div style="display: grid; grid-template-columns: 56px 1fr; gap: 16px; align-items: center; background: #f0fdf9; border-radius: 14px; padding: 18px 20px; border-left: 4px solid #028090;">
    <div style="width: 48px; height: 48px; background: #028090; border-radius: 50%; display: flex; align-items: center; justify-content: center;">
      <span style="font-size: 22px; color: white; font-weight: 800;">1</span>
    </div>
    <div>
      <p style="font-size: 20px; color: #1f2937; font-weight: 700;">具体的に伝える</p>
      <p style="font-size: 16px; color: #6b7280; margin-top: 4px;">「いい感じにして」ではなく「背景を青にして、ボタンを大きくして」</p>
    </div>
  </div>
  <div style="display: grid; grid-template-columns: 56px 1fr; gap: 16px; align-items: center; background: #f0fdf9; border-radius: 14px; padding: 18px 20px; border-left: 4px solid #00A896;">
    <div style="width: 48px; height: 48px; background: #00A896; border-radius: 50%; display: flex; align-items: center; justify-content: center;">
      <span style="font-size: 22px; color: white; font-weight: 800;">2</span>
    </div>
    <div>
      <p style="font-size: 20px; color: #1f2937; font-weight: 700;">一度に全部求めない</p>
      <p style="font-size: 16px; color: #6b7280; margin-top: 4px;">まず基本を作って、そこから「ここを変えて」と少しずつ改良</p>
    </div>
  </div>
  <div style="display: grid; grid-template-columns: 56px 1fr; gap: 16px; align-items: center; background: #f0fdf9; border-radius: 14px; padding: 18px 20px; border-left: 4px solid #02C39A;">
    <div style="width: 48px; height: 48px; background: #02C39A; border-radius: 50%; display: flex; align-items: center; justify-content: center;">
      <span style="font-size: 22px; color: white; font-weight: 800;">3</span>
    </div>
    <div>
      <p style="font-size: 20px; color: #1f2937; font-weight: 700;">遠慮しない</p>
      <p style="font-size: 16px; color: #6b7280; margin-top: 4px;">何回やり直しても大丈夫。AIは疲れないし、嫌な顔もしません</p>
    </div>
  </div>
</div>

---

# 改良するときの「魔法の言葉」

<p style="font-size: 20px; color: #6b7280; margin-bottom: 12px;">こんなフレーズを伝えるだけで、どんどん良くなります</p>

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 16px;">
  <div>
    <p style="font-size: 15px; color: #028090; font-weight: 700; letter-spacing: 1px; margin-bottom: 10px;">見た目を変えたいとき</p>
    <div style="display: flex; flex-direction: column; gap: 8px;">
      <div style="background: #f0fdf9; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #028090;">
        <p style="font-size: 17px; color: #374151;">「もっとカラフルにして」</p>
      </div>
      <div style="background: #f0fdf9; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #028090;">
        <p style="font-size: 17px; color: #374151;">「文字を大きくして見やすく」</p>
      </div>
      <div style="background: #f0fdf9; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #028090;">
        <p style="font-size: 17px; color: #374151;">「スマホでも使いやすくして」</p>
      </div>
    </div>
  </div>
  <div>
    <p style="font-size: 15px; color: #00A896; font-weight: 700; letter-spacing: 1px; margin-bottom: 10px;">機能を足したいとき</p>
    <div style="display: flex; flex-direction: column; gap: 8px;">
      <div style="background: #f0fdf9; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #00A896;">
        <p style="font-size: 17px; color: #374151;">「日付を自動で入れて」</p>
      </div>
      <div style="background: #f0fdf9; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #00A896;">
        <p style="font-size: 17px; color: #374151;">「入力し忘れたら教えて」</p>
      </div>
      <div style="background: #f0fdf9; border-radius: 10px; padding: 12px 16px; border-left: 3px solid #00A896;">
        <p style="font-size: 17px; color: #374151;">「データを保存できるようにして」</p>
      </div>
    </div>
  </div>
</div>

<div style="background: #f0fdf9; border: 2px solid #028090; border-radius: 12px; padding: 16px 24px; margin-top: 16px; text-align: center;">
  <p style="font-size: 20px; color: #028090; font-weight: 700;">ポイント：日本語でOK。専門用語は不要です</p>
</div>

---

<!-- _class: lead -->
<!-- _paginate: false -->
<!--
_backgroundImage: "linear-gradient(135deg, #028090 0%, #00A896 50%, #02C39A 100%)"
_color: #fff
-->

<div style="text-align: center;">

# では実際に体験してみましょう

<p style="font-size: 24px; opacity: 0.9; margin-top: 24px;">矢野さんの営業報告アプリデモの後、<br>皆さん自身でバイブコーディングを体験します</p>

</div>
