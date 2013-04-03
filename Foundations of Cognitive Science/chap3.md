# ロボットがフレーム問題に悩まなくなる日

## フレーム問題に関して

マッカーシー、ヘイズ「人工知能の観点から見た哲学的諸問題」で初出

次第に解釈が拡張され、人工知能から哲学の領域に言葉の主軸がシフトしてきた

### 変化する世界

人工知能（ロボット）の行動計画において、世界の変化にいかに対処するかという問題

ある出来事に関して、世界には変化する事柄と大部分の変化しない事柄が存在する。

形式的な演繹システムを用いると、出来事の帰結について公理からの演繹ですべてを推論しなければならず、莫大な数の公理が必要となる。

（公理：xをyで追い払う → (yがwの中にあったならば、yはwから出される)　など）

また、変化しないことに関しても同様に公理からの演繹により知識獲得する必要がある。こうした導出の基礎となる公理が**「フレーム公理」**であるが、これはさらに莫大なものとなる。

あらゆる出来事について世界に関するすべての公理（知識）を用いなければならないのか？

### フレーム問題の典型的説明

デネットによる有名な説明

時限爆弾の仕掛けられた部屋の中にあるバッテリーを救出するというタスクをロボットに与える

#### ロボット 1

意図した因果しか扱うことの出来ないロボット

（引っ張ったら、動くといった公理を用いて）バッテリーが載っているワゴンごと引っ張りだしたら、爆弾もワゴンに載っていて爆発してしまった

もともと意図されていない副次的効果を演繹する能力がなかった

#### ロボット 2

常にあらゆる副次的効果を考慮するロボット

ワゴンを引き出しても部屋の色が変わらない、ワゴンを引けば車輪が回転する、など関係することも関係しないこともすべて考えようとしている間に爆弾が爆発してしまった

扱うことの出来る問題にはキリがなく、目標に対する帰結の関連性に無頓着であった

#### ロボット 3

演繹した帰結を目下の目標との関連性で分類し、関係ないものは無視するロボット

無関係なものを無視するため、関係するか否かを判別する処理をしなければならず、結局根本的解決にはならなかった

### フレーム問題の本質

#### (i) 端的な無視

関連する知識と関連しない知識を区別することに加えて、関連しないことをあえて個別に判別せずにそっとしておけることが必要

理想的な行為者としては、行為ごとに知らなければならないことのすべてをちょうどぴったりと、自分が処理できる時間と労力の範囲内で知ることの出来るメカニズムが存在することになる

**「〈何を考えなくてもいいか〉を考えなくても、考えなくていいことをいかに考えずにすますか」**、つまり端的な無視が本質的な問題

#### (ii) 関連性

ある知識が、現在の目的と関連するか否かをそもそもどうやって正しく判定することが出来るのか？

知識と知識、情報と情報、信念と信念との関連性は、文脈依存で決まる全体論的性質である

"anything can be related to anything"

あらゆるものが互いに関連性を持ちうる情報の組織化を無限の計算量を用いずにいかに行うか

#### (iii) 規則と例外

例外：築かれたフレーム、スキーマ、スクリプト、プロトコルで考慮されない事態

基本的にフレームは場合によって細部をその場の状況に合わせることで、だいたい同じように振る舞うようにする

ゆらぎの範囲（バッテリーがカゴに入っているかワゴンに乗っているか）と、（爆弾がワゴンの上にあるというような）とんでもない例外とを区別しなければならない

例外としてどのようなものがどれくらい存在するかは事前に計算出来ない

形式的な演繹システムでは、「特別な事情」は明示的に列挙しなければふつうのゆらぎと区別できないが、これは不可能である

フレーム問題への根本的な解決はもたらされていないが、以降は古典的計算主義の範囲では解決は不可能とする議論、コネクショニズム下でいかに可能とされているかの議論、それでもまだ解決されていない問題と今後の展望を順に述べていく。

## 古典主義でのフレーム問題の解決不可能性

ホーガン、ティーンソンによる古典主義の特徴付け

1. 知的な認知は、構造的に複雑な心的表象を用いる
2. 認知過程は、これらの表象の構造に左右される
3. 認知過程は精確な規則に合致し、コンピュータプログラムの形でも書ける
4. 多くの表象は統語論的構造を持つ
5. 認知状態の推移は物理的手段で実際に計算可能な認知推移関数に合致する

我々は絶え間ない認知推移の器、計算デバイスとして解釈される。

それでは認知推移関数はいかにして計算されるか？ ... 表象が変化する媒体を担う

外部の情報を担う（意味論的内容を持つ）と同時に、その集まりにおいて心的状態を構成する認知状態である。

認知状態相互の推移関数は記号としての表象への形式的操作として計算されるとする。

### 表象

人間の認知過程が環境世界の複雑な情報を処理して組織化された理論的認識まで至ることを考えると、表象を用いることが必要である(1)

統語論を持った表象の概念は、知識や意味論といった上位レベルと神経科学的下位レベルから独立した中間レベルの対象として議論されてきた。

自然言語そのものでもなく、物理的実体が観察されるわけでもない以上、「うまく説明できるか」をもって表象概念の正当性は示されうる

表象がそもそも認知過程に要請されるのは、信念や知識が時間的に整合性を持つことを説明できるためである（形式的操作は整合性に関する健全性を保証し、認知過程は表象の構造に依存するとする）

というのは、我々はコンピュータ言語のように意味論が統語論に依存するような形でしか因果的効力の発揮を説明できないからである(2)

従って認知的過程は表象を扱う精確な規則となるはずであり、コンピュータプログラム(論理式)の形で書くことができるとするのは自然なことである(3)

表象は複雑で意味論的な整合性を持ち物理的なメカニズムで説明の出来るものである必要がある ... フォーダーの思考の言語仮説により、自然言語のような統語論的構造が仮定されるように(4)

認知過程がプログラムとして見られる規則によるのであれば、トータルな認知過程の推移もやはり複雑であろうと実際に計算可能な関数として理解できる（数学的計算可能性と言うよりも、物理的計算可能性に属する）

### ホーガン、ティーンソンによる古典主義批判

以上の古典的計算主義の前提のうち(3), (5)を否定する

つまり、思考の言語仮説を指示し表象の統語論的性質を仮定しつつ、それらの実装は統語論的操作（プログラム）ではなくニューラルネットワークにおける並列分散処理を指示し、数学的には力学系として理解するような異端的なコネクショニズム

#### 規則では我々の認知活動をうまく説明できない

ある規則における例外を処理するには、例外を含んだ高位の規則が要請される

規則のメタ規則のメタ規則の...と、余すこと無く説明できるような高位の規則を考えるのは正当だろうか

また、認知を規則としてみなすことは、我々のほとんどの行動は問題解決活動ではないということからも怪しい

仕事中コーヒーカップに手を伸ばすタイミングを決定するような内的規則は存在すると考えるべきか？

規則を無尽蔵に生産するようなメカニズムを擁する規則、すなわち万能型知性を前提しないと認知を説明できない

万能型知性は例外の無い人生の規則とでも呼ぶべきものとなり、意味不明である

**フレーム問題は知性という枠を超えて、生存するシステムを扱う理論の次元ではないか？**

#### 一般的な形での関連性の問題

関連性について適切にとらえるためには、全体論的な情報処理が要求される

古典主義者であるフォーダーによってもこの点は批判がされている

認知モジュール理論では、各モジュールは高速かつ高効率に処理を行える代わりに、独立していて他モジュールを参照できず、また入力を疑いなく処理して中央システムに出力する（**モジュールの領域限定性**）

cf. 水槽に差し入れた真っ直ぐな棒が水中で曲がって見える現象

モジュールは統語論的構造に従って処理を行い、一方で中央システムは統語論的構造は持たないと考えられている

ある主張を表す表象の統語論的特徴はモジュール内でローカルに処理されるので、文脈（信念システム）可感的でない一方で、グローバルな関連性に関する推論は文脈可感的な性質に依拠して行われる

この問題を解決するためには、中央システムを合わせて信念システムの全体に統語論的特徴が与えられる必要がある（弱い計算主義）

しかし、これではドメインが大きすぎて心理学的モデルとしては現実的ではない（結局モジュールが解除されてしまうので、出来事に対して何が起こるのか分からなくなってしまう）

コネクショニズムでの解決は不可能とするフォーダーの立場では、まさに全くのミステリーとして残ってしまっている

## コネクショニズムのアプローチ

### 古典計算主義からコネクショニズムへ

1. 古典計算モデルは領域限定的であることが本質的（全ての例外を網羅する万能型知性はナンセンス）
2. 従って、古典計算主義は文脈非可感で効率的に処理を行う認知モジュールの説明には妥当する
3. 一方、認知過程の中心は非論証的推論が占める（アブダクション、日常的推論）
4. 非論証的推論は本質的に文脈可感的である
5. 古典主義は認知仮定の中心的な部分をうまく説明できない

少ない情報から世界の姿を補間し、新たな情報からそれを調整し、維持し、行動プランを立てる、時間的制約の中で最善の判断をするといった認知らしい中枢部分は古典主義では全く説明が出来ない

ここでコネクショニズムのアプローチが提案される。

"表象とは何か"の議論は、フレーム問題のような具体的な問題への説明の成否を通して判断しなければ神学論争に終わる可能性がある。
よってここではコネクショニズムと古典主義の論争には踏み込まない。

### スキーマ

ラメルハートとスモーレンスキーによる構築、**部屋を表現するネットワーク**を題材とする。

古典的CNの特徴として（すでに何度も説明しているが）計算の並列性、表象の分散性、重み付けによる学習が挙げられる。

スキーマのネットワークの特徴は、ネットワークの動作を**「入力値から出力値への変換」**ではなく、**「ある入力に対してネットワークが安定する仮定」（relaxation）**と見ることである。

〈制約-満足ネットワーク〉と広くカテゴライズされるネットワークとなる。

#### ネッカーキューブとネットワーク

ネッカーキューブ解釈に対応する２つのサブネットワークの結合で表される。

異なる解釈の同じ頂点を意味するノード同士で抑制し合い、同じ解釈の隣接ノード同士で強め合う。

最適状態は右向きキューブか左向きキューブかの択一であり、中間状態は不安定。

結合の強さをうまく調整すれば、ネットワークが安定した際にどちらの解釈かに固定される。

#### スキーマのモデル

家財道具のセットから５種類の部屋のモデルを構成する。

家財道具40個の間で、例えば本と本棚は強め合う、ベッドと浴槽は弱め合うといった〈制約-満足ネットワーク〉を構成する。（被験者に５種類の部屋のイメージをアンケートして結合パラメータを決定する）

このネットワークに生起する部屋のスキーマについてまとめる

1. スキーマは生成する

不安定な状態の部屋ネットワークに、「オーブン」などを強める特徴的な入力を行うと、自発的に安定化を続けて最終的に台所のプロトタイプに自発的に到達する。

2. スキーマは類似する

40次元空間に適応度で高低パラメタを与えると、例えば2次元で切り取ると幾つかのピークが見つかる

こうしたピークが各スキーマに対応するが、ピーク間の距離がスキーマ同士の距離、地形に対応する。

3. スキーマは柔軟である

いくつかプロトタイプとなるスキーマに例外的な条件が混ざっていたとしても、自発的に安定性が高まるようにネットワークが挙動し、既存のプロトタイプに帰着するなり、新しい変則的なスキーマが出現するなりして安定する

4. スキーマは構造を持つ

スキーマの内部には小スキーマが存在しうる。

例えば窓とカーテンのペアは強め合うことで様々な大スキーマの中に埋め込まれて構成要素となる。

5. スキーマは定義的情報ではない

スキーマは「台所とは○○である」といった定義をしているのではなく、可変的な結合にほかならないので確固たる知識からあやふやな信念まで色々なレベルの情報を表現できる。

定義に近い固いスキーマは地形勾配が急になるし、あやふやならなだらかな地形となる。

部分的に厳格な小スキーマを持つゆるやかな大スキーマといったものも考えられる。（冷蔵庫を持たない台所もある）

#### コネクショニズムはフレーム問題を解決するのか

1. 規則性と例外の問題

そもそも規則が与えられるわけではない以上「例外」を定義する必要もない。

スキーマから離れた入力がなされても自発的な調整によって安定化されることで例外に対処されている

2. 「無視」のパラドックス

規則性が定義されない以上、問題領域が限定されないので無視の問題も生じないだろう。

例えば「窓」「カーテン」のペアは、普通ともに0かともに1を取り、その存在は適応度に影響を与えない（無視される）

一方で、どちらかだけが1という特殊なケースでは、ネットワークの非安定性に強く寄与し、部屋の様子を大きく変化させる要因として機能する。

このように背景要因と前景要因とのなめらかな移行が実現されている。

計算論的に考えて「無視」の賢い実装方法は、常に全てのものを計算に関わらせつつ、その計算をあからさまに行う必要を廃することである

3. 何と何が関連するのかの問題

「すべてのものがすべてのものと関連しうる」という特徴は、ネットワークにおいて家財道具ユニットが互いに結合されているという様式によって実現されている

同時に、各家財道具は文脈非可換的に存在しているのではなく、他の全ての要素との関連性、それ自身の興奮度によってスキーマによって異なる現れ方をしている。

例えばスキーマAとスキーマBである家財道具が同じ興奮度となっているとしても、それを強めたり弱めたりした時の影響は異なる。

関連性の問題は、結局すべての表象が計算過程で常に互いに関連しあうという認知メカニズムによって可能になり、そのモデルとしてスキーマの生気したネットワークのような全結合ネットワークが挙げられる。

また、スキーマは階層性を持つことにより、家財道具のようなユニットを固定的に考える必要もない。

（※疑問：ユニットは結局どうやって生成すると考えればいいのか？例えば家財道具のネットワークは40個を選んだ段階で明確に有限個の大きさに制約されている。この恣意性を解決するには非離散的でかつ全対全結合するネットワークが必要になるのではないか？結局最下層には何が位置づけられるのか？）

## 自然知性

コネクショニズムのアプローチに関する幾つかの欠点

### スケーラビリティの問題

フレーム問題は莫大な量の知識や経験が関連する課題において顕在化するものであるから、小規模な問題で柔軟な認知モデルが構成できることはそのままフレーム問題の解決を意味しない。

例えばラメルハートのネットワークは大規模なデータ領域にそのまま拡張できるのか？

ヘイスレイガーとファン・ラパードの文法解析ネットワークへの分析
 ... CNの一般化能力は部分的なものにすぎないのではないか。法則による裏打ちを確認することは出来るのか？

言語構造の分散表象はもっと大きな分散表象構造に組み込もうとすると束縛関係が損なわれてしまう。これは解決可能か？

### 情報の質に関して

フレーム問題が顕在化するのは、統語論的な構造を持たず様々な情報を集約する中央システムにおいて。

１つのネットワークを複数の問題領域の入力を同時に処理できるようにすることは本当に出来るのか？

少なくとも、ある領域のために学習されたネットワークが他の問題のために利用できることは示せないと我々の認知過程を記述することは絶対にできない。

結局、**ネットワーク統合問題**とはコネクショニズムの衣をかぶったフレーム問題そのものなのではないか？

領域限定であれ発達の仮定を真に実現するためにも、様々な経験を学習に生かさなければならないので同じ問題をはらむ。

### 自然知性と感情

出発点の確認：**フレーム問題とは本来、現実のワイルドな環境下で実際に行為をするときに出現してくる問題ではないか**

シミュレーションは必然的に有限の問題しか包有できない以上、真にフレーム問題を扱うことは原理的に不可能

時間と資源の有限性の中で行為する、という制約（上手い計算と下手な計算の区別）こそ本質的

従って、フレーム問題の解決の手立ては現実に振る舞う自然知性一般に見出すべきである

我々は無限の計算能力を持つ天使ではない、という事実を真剣に受け止めて手がかりを探すべきではないか？

オートリーとジョンソン-レアード

- 目的と現実とのギャップ
- 感情の必要性
- アブダクティブな推論を発動させる要因

もっとも、感情の存在＝アブダクティブな推論の必要十分条件、とはっきりしているわけではないので、感情こそヒューリスティクスであるという主張も根拠には欠けている

純粋理性で埋められないギャップを、敢えて情報閉鎖してしまう（感情による）ことで埋めることはフレーム問題を扱う自然なやり方の１つ（スーザ）

では、情報閉鎖してもなおアリよりも我々が賢いこと、無差別に情報を削減しているわけではないことはどうやって説明する？

結局いかに適切な情報閉鎖を行うかということを考えると、結局議論としては前進したとは言えない

感情と計算システムの相互作用によって認知-行為のメカニズムを具体的に描けていない以上、議論は詰まっていない。

### フレーム問題の解決へ

1. 感情の機能の徹底した洗い出し

シミュレーションが容易な古典的計算論的部分は多くが明らかにされてきたが、生存システム全体というシミュレーション不可能な領域についてはそれが何であるかというレベルで手付かずである

例えば感情の機能、意識、クオリアなど

まずは心理学的現象としての感情が生存にいかなる貢献を果たしているかを検証しなければならない

2. マクロなレベルとして現れる機能が実際にはどのような作用として現れているか

伝統的にマーの「計算論的レベル」「表現・アルゴリズム的レベル」「ハードウェアのレベル」という三層で認知は理解されてきたが、フレーム問題に対処する上では異なる枠組みを導入する必要があるかもしれない

ロボットがフレーム問題に悩まなくなることとは、アリ（極端な情報閉鎖）と天使（不可能な万能計算能力）の間に自身の存在論的位置を見出した時であると言い換えることが出来る。
