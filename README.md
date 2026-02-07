# Workout Compass（仮）

筋トレの「目標設定 → ジム予定 → 当日のメニュー（混雑Plan B）→ 忘れ物チェック → 体調 → 記録 → 振り返り（改善点）」を一つにまとめ、
成長（伸び）を実感しやすくし、継続しやすくする記録アプリ。

このアプリの強み：
- **部位テンプレ（胸/背中/脚/肩/腕）**で予定作成が速い
- **混雑時Plan B**が最初から用意されている
- **忘れ物チェック**が部位に紐づいて表示される
- **前回の改善点が次回開始時に出る**
- **1周分の予定ブロックを期間指定で一括生成**できる
- 行けなかった日は **3択で回復**できる（軽い代替 / 次回に追加 / 全体スライド）

---

## Problem（何が面倒？）
- 無料の筋トレ記録アプリは入力が多く、目的（成長実感）に直結しにくい
- インターバルや体調、混雑による「代替メニュー（Plan B）」が記録・運用しづらい
- 反省点・改善点が散らばっていて、次回トレで見返せない/活かせない
- 「いつ行くか・何をするか」が曖昧になり、継続が途切れる
- 忘れ物（グリップ/ストラップ等）でパフォーマンスが落ちる

---

## Solution（何を作る？）
計画（いつ行く・何をやる・持ち物）と実行ログ（重量/回数/体調/インターバル）、
振り返り（改善点）を同じ画面導線で完結できる“軽い”筋トレ記録アプリを作る。

ユーザーごとに **部位ローテ（順番）** と **休みルール（Rest Rules）** をカスタマイズでき、
さらに「1周分の予定」をブロックとして保存し、**期間指定（例：4週間）**で未来の予定を一括生成できる。

---

## Features（5つまで）
1. **目標設定**（年/月/週/日）＋進捗の見える化（伸び・継続）
2. **ジム予定（手動）＋期間指定のブロック一括生成**（ユーザーごとにローテ/休みルールをカスタム）
3. **テンプレメニュー（部位別）＋混雑Plan B**（器具が空いてない時に即切替）
4. **実行ログ**（セット/重量/回数/インターバル/体調・睡眠・痛み）＋最小入力
5. **振り返りメモ**（改善点・次回の注意）を次回開始時に自動表示＋行けなかった日の回復3択

---

## Workout Templates（部位別テンプレ）
胸・背中・脚・肩・腕の5カテゴリにテンプレを用意し、
予定を作ると「今日のメニュー」「混雑時のPlan B」「持ち物チェック」が自動で出る。

### Chest（胸）
**Default Menu**
- Bench Press
- Incline Dumbbell Press
- Cable Fly
**Plan B**
- Bench → Dumbbell Bench / Machine Press
- Cable Fly → Pec Deck
**Carry Checklist**
- Gear: グローブ（必要ならリストラップ）
- Nutrition: トレ前軽食 / プロテイン
- Clothes: 着替え

### Back（背中）
**Default Menu**
- Lat Pulldown / Pull-ups
- Barbell Row / Seated Row
- Face Pull
**Plan B**
- Row系 → Machine Row / One-arm DB Row
- Pulldown → Assisted Pull-up
**Carry Checklist**
- Gear: リストラップ or パワーグリップ / グローブ
- Nutrition: トレ前軽食 / プロテイン
- Clothes: 着替え

### Legs（脚）
**Default Menu**
- Squat / Leg Press
- Romanian Deadlift
- Leg Curl
**Plan B**
- Squat → Leg Press / Smith Squat
- RDL → Back Extension / Hamstring Machine
**Carry Checklist**
- Gear: （使うなら）ベルト / ニースリーブ
- Nutrition: トレ前軽食 / プロテイン
- Clothes: 着替え

### Shoulders（肩）
**Default Menu**
- Overhead Press
- Lateral Raise
- Rear Delt Fly
**Plan B**
- OHP → Machine Press / DB Press
- Lateral → Cable Lateral
**Carry Checklist**
- Gear: グローブ
- Nutrition: トレ前軽食 / プロテイン
- Clothes: 着替え

### Arms（腕）
**Default Menu**
- Biceps Curl (DB/Bar)
- Triceps Pushdown
- Hammer Curl / Overhead Extension
**Plan B**
- Pushdown → Dips / Cable variation
- Curl → Machine Curl / Cable Curl
**Carry Checklist**
- Gear: グローブ
- Nutrition: トレ前軽食 / プロテイン
- Clothes: 着替え

---

## Rest Rules（休みルール）
単純な「毎N日」ではなく、部位ごとの休養ルールで予定を生成できる。

**Example（自分のルール）**
- 脚（Legs）の翌日は休み
- 肩（Shoulders）の翌日は休み

生成されるサイクル例：
Chest → Back → Legs → Rest → Shoulders → Rest → Arms → (repeat)

---

## Block Generation（期間指定の一括登録）
- ユーザーは1周分の部位ローテ（例：胸→背中→脚→休→肩→休→腕）を「ブロック」として保存できる
- 生成時に「開始日」と「期間（例：4週間）」を指定し、未来の予定を一括で作成できる
- 生成された予定は個別に編集/削除できる（ブロック由来の予定だけ一括削除も可能）

### Example Schedule（2週間イメージ）
Mon: Chest  
Tue: Back  
Wed: Legs  
Thu: Rest  
Fri: Shoulders  
Sat: Rest  
Sun: Arms  
Mon: Chest  
Tue: Back  
Wed: Legs  
Thu: Rest  
Fri: Shoulders  
Sat: Rest  
Sun: Arms  

---

## Missed Day Recovery（行けなかった日の扱い：3択）
予定日にジムに行けなかった場合、ユーザーに次の3つを提示してローテを回復する。

1) **Light Alternative（その日にできる軽いメニュー）**
- 自宅/短時間でできる軽めの代替メニューに切り替えて、その日の予定として記録できる

2) **Add to Next（次のジム日に軽い追加入れ）**
- 次のジム日に、スキップした部位の軽いメニューを追加して消化する（メインは予定通り）

3) **Slide All（予定をそのまま全体スライド）**
- いけなかった日のメニューを翌回に持ち越し、以降の予定をすべて1つずつ後ろへずらす（Rest Rulesも維持）

---

## Growth Signals（成長の可視化）
- 種目ごとの重量/回数推移（例：Benchのトップセット）
- 週間回数・連続継続日数
- 体調（睡眠/疲労）とパフォーマンスの関係のメモ
- 前回の改善点 → 次回の実行で反映できたかチェック

---

## Tech Stack
- Backend: Java / Spring Boot
- DB: PostgreSQL（開発はH2でもOK）
- Frontend: Thymeleaf（最短） or React（余裕あれば）
- Auth: まずはログインなし → 後でGoogleログイン等
- Deploy: Render / Railway など（無料枠でOK）
- Tools: GitHub Projects（タスク管理）

---

## Milestones（Week1〜4で何を作る）
### Week 1：MVP設計 + “最短で動く”骨組み
- 画面の流れを決める（Plan→Start→Log→Review）
- データ設計（目標、予定、テンプレ、チェックリスト、メモ）
- README更新＋スクショ用の簡単な画面モック（手書きでもOK）
- リポジトリにIssue/Project作成（タスクを見える化）

### Week 2：計画（予定・テンプレ・ブロック生成）
- 部位ローテ（順番）とRest Rules（脚/肩の翌日休み）を保存
- 予定の手動作成（部位テンプレ適用、持ち物チェック表示）
- ブロック保存 → 期間指定で未来の予定を一括生成
- 生成された予定の一覧表示＆個別編集

### Week 3：実行ログ + インターバル
- セット/重量/回数の記録
- インターバルタイマー（開始/停止/履歴）
- 体調（睡眠/疲労/痛み/気分など）をワークアウトに紐づけて保存
- 予定に done / skipped を付けられる

### Week 4：振り返りUX + 欠席回復 + 成長可視化
- 振り返りメモ（改善点/次回の注意）入力
- 次回開始時に「前回の改善点」を自動表示
- Missed Day Recovery（3択）実装（軽い代替 / 次回追加 / 全体スライド）
- 伸びの可視化（重量推移、継続日数、週間回数）
- デプロイ＋デモ用GIF/スクショをREADMEに追加

---

## Future Ideas
- 目標や計画の作成をAIでサポート（提案・調整・リマインド文生成など）
- 曜日固定（Mon=胸など）や週N回ペースの柔軟な繰り返し
- 混雑状況や体調に応じてPlan Bを提案
- スキップが続いたときの自動リスケ（未消化を次回へ繰り越し）

---

## Status
- Start Date: 2026-02-06
- Current: README完成、画面導線とデータ設計を確定中
