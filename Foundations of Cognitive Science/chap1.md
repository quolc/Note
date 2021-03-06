# 心は(どんな)コンピュータなのか

**「心は計算機であるとしたら、どんな計算機なのか？」**

## 計算主義

計算主義：古典計算主義＋コネクショニズム

いずれも、心の内部メカニズムに目を向ける

20世紀前半の行動主義全盛へのアンチテーゼとして成立

### 認知関数と表象

計算においては、**「どんな関数が計算されているか」** **「何が操作されて計算過程が進んでいるか」**の二点が重要

計算主義では、認知過程は表象の操作関数の計算として考えられる

### アーキテクチャ

基本的操作・関数の定義域と値域が表象であるようなアーキテクチャを認知アーキテクチャという

計算主義者の問うべき問題：「こころの持つ認知アーキテクチャはどのようなものか」

２つの研究プログラムとして、古典的計算主義とコネクショニズムがある

## 古典的計算主義の認知モデル

古典的計算主義での認知モデルを整理する

### 1. 心は形式システムである

形式システム
... 離散的対象を推論規則に従って変形することで計算が行われる

### 2. 統語論的構造を持つ表象

* 表象の合成性

表象は原子的表象からsyntacticに構成される. 意味論も構文論的構成によって一意に決定する

* 表象処理の統語論的感受性

表象への操作はその統語論滴構造によって決定する

### 3. 思考の言語仮説

1, 2の条件を満たす典型は言語であり、心のなかに言語のような表象の存在を仮定する

思考の言語で描かれた文のsyntacticな変形によって心的計算がなされる

### 4. 統語論的エンジンとしての心

心は表象の統語論だけによって制御される

## 認知研究の３つのレベル

計算主義での記述に関するマーによる提唱

* 計算論的レベル ... 何をするか
* アルゴリズムレベル ... どうするか
* 実装レベル ... 具体的な仕組みはどうなっているか

各レベルは上下のレベルを制約するが、決定はしない

古典主義は上位から下位への制約を重視し、コネクショニズムは実装レベルから上位レベルの実現に長ける

## コネクショニズムの認知モデル

### 1. コネクショニスト・ネットワーク(CN)の構造

いわゆるニューラルネットワーク. （詳細は省略）

結合の様式によって様々な種類が考えられる（階層型ネットワーク、全結合型ネットワークなど）

### 2. CNは何をするか

例えば三層ネットワークでは、入力層から隠れ層を経て出力層へ興奮を伝播する

行なっていることはベクトル変換に他ならない

### 3. 学習と訓練

CN各ユニットへの入力重みの調節によって、望ましい出力を行うように学習させられる

教師あり学習と教師なし学習がある（学習則, ヘブ則やコホネンのアルゴリズムが有名）

ローゼンブラットのパーセプトロンはXORを計算出来ないことから一時期関心が離れるが、
ラメルハートのバックプロパゲーション（教師あり学習）や三層以上ネットワークのXOR計算可能性の証明により再燃する

### 4. CNが行う処理の特質

* 一般化能力 ... 性別判断など新しいデータの入力に対して良い振る舞いをする

* 劣化入力耐性 ... 多少のノイズや欠損のあるデータでも処理できる

* 全体論的処理 ... どんな処理でもすべてのユニットが関与し、分業をするわけではない

* 非アルゴリズム的処理 ... 問題ごとに明示的なアルゴリズムによって処理を行うわけではない

* パターン認識や柔軟な制約問題, 近似的解法など古典的手法が不得意とする問題に秀でる

### 5. 分散表象

表象（CNの興奮パターン）を構文論的に分解することは出来ない

## 古典主義とコネクショニズムの論争

両者とも表象に関する計算として認知を捉える点では共通しているが、表象と処理の見方に差がある

今日まで、古典主義からコネクショニズムに様々な批判が寄せられている

### 1. 体系性に関する批判

フォーダーらによる

認知能力に備わるべき生産性と体系性をコネクショニズムは説明できないとする議論

* 生産性

> B think A
  C think that B think A
  D think that C think that B think that A

という具合に、人間はいくらでも表象を算出することが出来る

また、A loves BとB loves Aのように関連しあった表象を常に抱くことが出来る

* 体系性

「P∧Q∧R → P」を推論できる人は「P∧Q → P」も推論できるというふうに、関連し合った処理は共通して出来るべきである

フォーダーらは、思考の言語仮説（統語論的構造を持つ表象）によってこれらの規則性を説明できるとする

また、コネクショニズムが規則性を説明できたとしても、その際に統語論的構造を持ちだした段階で古典主義の実装を示しただけになる、とする

### 2. ありうる反論

フォーダーらが前提とする規則性は実は成立しない場合が多い（子供で顕著）

認知の必要条件として規則性を要請するのは過剰ではないか？

### 3. 古典主義モデルの実装としてのCN

古典主義モデルを完全に実装するCNを作ることは、本当に古典主義に埋没するのか？

上述の三層モデルは相対的であることに注意（計算論的レベルは実装やアルゴリズムに優越するわけではない）

認知機能での性質に本質的な関連性を持つのがどのレベルであるかは明らかではない

### 4. RAAMとチャルマーズの実験

#### RAAM（Recursive Auto-Associative Memory）

ポラックによるメモリの働きをする三層ネットワークで、構文論的構造（回帰節）を持つ入力を分散表象として記憶できる

13個の文からなる訓練セットで学習させ、訓練セットに属さない12個の文も構造を記憶し正しく再現できた

処理できる階層には限界がある ... 人間の生成性も限界があるので大きな問題ではない

あくまでも統語論的構造を持った文を圧縮表象として記憶するメモリでしかなく、処理は出来ない

#### チャルマーズの実験

RAAMの変形により、文を能動態から受動態に書き換えるCNを構成

60個の入力文による学習で20個の文を100%の精度で処理し、高い一般化を示した

これでフォーダーの議論に反駁したと主張できるか？

CNが統語論的構造を処理できたことに関して何らかの説明が必要！

### 5. 統語論的構造を持つ表象と思考の言語

認知の規則性の説明が本質的に依拠しているのは、「表象の合成性」と「処理の統語論的感受性」の二点

ゲーデル数を用いた処理を考えると、統語論的構造を持たない表象を用いて論理式の操作と等価な推論ができる

* 「複合的表象は統合論的な構造の情報を持っている」

* 「心的計算における表象への操作は、その表象が持つ統語論的構造についての情報に依存して決まる」

と認知の規則性の条件を言い換えれば、思考の言語は唯一の選択肢ではないことがわかる

統語論的構造の顕在性 ＝ **連鎖的合成性** 表象のはoptionalな性質である

一方でゲーデル数の持つような連鎖的合成性を持たないが統語論的操作が可能な性質は **機能的合成性** と呼ぶ

### 6. フォーダーの議論は成り立たない

RAAMの分散表象は連鎖的合成性を持たないが、機能的合成性を持つ

従って、認知の規則性を説明するのに要請される条件を満たすと考えられる

それではCNは処理の観点から明示的構成要素を持つからと古典主義に回収されるとしてよいか？

上述のように、**「どのように処理しているか」**の点でCNと古典主義は依然として異なる

* 古典主義：因果的効力は表象に関する規則がシステムに実装されている

* CN：表象に関する規則はシステムではなく学習されたデータとして実装されている

という大きな差が存在するので、CNを古典主義の一部とするのは甚だ不当である

### 7. 最後の問題

コネクショニストに残った大きな問題として、CNによる規則性発現の必然性を説明することが挙げられる

規則性を表すCNを構成することが出来る一方で、反規則的なCNを構成することも出来てしまうのではないか？

この疑問へは次のように反論できる

* 古典主義アーキテクチャから規則性を導けるのは、推論規則を恣意的に導入した場合のみである

* 古典主義でRabからRbaを導けるというのはそもそもおかしくないか、そういう過程はすぐには出てこない

* フォーダーらの科学的説明に関する理解がおかしいのではないか。

被説明項が必然化される根拠を、それが理論言明から恣意的過程を置かずに演繹されることに見出そうとするのは、工学や生物学のモデル化による説明の方法論と矛盾するのではないか。

## コネクショニズムと思考の言語

### 1. 思考の言語仮説

古典主義とコネクショニズムを合わせて、統語論感受性を満たす（機能的合成性を持つ）表象を用いる、
思考の言語仮説のサブカテゴリとしてみなす分類法があるが、シンボル表象に対してイメージ表象などの存在も考えると適当とは言い難い

* 強い思考の言語仮説（連鎖的合成性を要請）
* 弱い思考の言語仮説（機能的合成性を要請）

と区別することにする

コネクショニズムは弱い思考の言語仮説と両立可能で、規則性を説明できるというのが上述の理論

### 2. 弱い思考の言語仮説とコネクショニズム

コネクショニズムは本当に（弱い）思考の言語仮説を受け入れなければならないのか？

#### 機能的合成性はタスク相対的である

RAAMはそもそも、統語論的構造を持つ入出力に対して、
統語論的変形というタスクを行うためのシステムで用いられているからこそ統語論的構造を持つといえる

岩と機雷を区別するシステムでは、入出力に統語論的構造が無いのでCNは統語論を持たない

分散表象が合成性を持つか否かはタスクによって決まるものであり、コネクショニズムに普遍的に備わる性質ではない

#### 機能的合成性と連鎖的合成性の差異

連鎖的表象では、統語論が明示される
→ 機能的基準から独立して同一性基準を取り出すことで、機能から独立して構造情報を保持できる

機能的表象（分散表象）では第二の基準を持てないので、ネットワーク内で果たす役割によってしか構造を同定できない

特に回帰的ネットワークでは同じ活性化パターンでも同じ機能を果たすとは限らないので致命的

#### 弱い思考の言語仮説はあまり意味がない

強い言語仮説が認知理論の基本テーゼでいられるのは、同一性基準の二重性（機能性＋連鎖性）による

一見言語を使っているようには思えない知覚や顔認知などすべての認知処理で、言語的構造を持った表象が操作されている

「言語的構造を持った表象」は同定されなくては理論の意味が無い

連鎖的合成性を持つ古典的表象ではそれが可能（連鎖的同一性による）だが、機能的合成性だけでは構造が処理に依存するので実質的な意味がない

*RAAMが機能的合成性を持つのは、あくまでも入力に連鎖的合成性を持つ文（のコード）が入力された時だけ*

#### 結論

* 分散表象がある種のタスクで機能的合成性をもちうるということは空虚ではないし、コネクショニズムの意義を擁護できる

* しかし、機能的合成性を持つ表象の統語論的処理ですべての認知過程を理解すべき、という弱い思考の言語仮説は採用する意味が無い

### 3. コネクショニズムが思考の言語仮説を脱出するには

いくつかの方向性が提案されている

#### (1) 言語は表象ではないかもしれない

カミンズ　表象のピクチャ理論

例えば地図であれば、地図の構造と地形とに一対一の対応関係がある（homomorphic）ことがポイント

「すべての自然な表象の基礎をなすものは、こうした構造間の同型性である」という主張

自然言語は意味する構造との間にこのような同型性は成り立たない ... では自然言語は何なのか？

→ 自然言語はトリガーとして類似の思考をコード化している図的表象を相手の脳内に引き起こす

#### (2) 思考のファシリテータとしての自然言語

* 認知とは表象に対する操作である

* 言語は表象ではない

* ∴ 言語は認知の媒体ではない

言語のような構造化した媒体なしでどうやって抽象的思考をやるのか？

→ 思考のファシリテータ、外部記憶としての言語（筆算を代表とする）

#### (3) 自然言語の内面化

さらに、ファシリテータとしての自然言語の利用を内面化（内語の獲得）することで高度な思考・認知が可能になる

#### (4) 手続き的知識の集積としての思考

思考は次のようなものとして整理できる

* 高度で抽象的な思考は、自然言語の外部記号の補助によって初めて可能になる

人間の認知能力の本体とは、**外的な**統語論的構造を持ったアイテムを相手に作業を行う手続き的知識である

従って、認知システム自体には構造は要らない

* 脳が外的自然言語を内面化する

紙やペンがなくとも複雑な思考ができるよう、外的な自然言語を内面化する

それは不完全であるので、非常に複雑な事柄には外部記号の補助を必要とする

* 内面化された言語は相変わらずファシリテータである

必要に応じて脳に分散表象を生じさせ、認知活動を引き起こすトリガーとなる

* 人間の認知の規則性はフォーダーが考えているほど普遍的ではない

規則性を示す認知タスクはほとんどが自然言語に関わるものである

規則性は認知自体の特性ではなく、自然言語自体が構造を持つのである

**コネクショニズムはそもそも統語論的構造を持つ内部表象を持つ必要は無いかもしれない**（ラジカルなコネクショニズム）

「我々は言語を使って考えるのであり、言語において考えるのではない。」（オブライエン, オピー）
