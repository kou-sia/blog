# 面接官のコツというか感じたこととか

**前置き**  
なるべく本来の実力を発揮してもらいたいので会話の中で様々な工夫を行っています。  

面接で大切なのは「出すべき内定を出すこと」と「出さないべき内定を出さないこと」の2つです。  
私は後者を重視しています。  

この記事に登場する会話はフィクションです。  

## 更新日

- 作成日: 2024/04/29
- 最終更新日: 2024/05/19

----

面接官として20回ほど、新卒中途問わずエンジニア/マネージャーの採用面接をおこないました。  
そこでわかった事を整理します。  
面接を受ける側から見ても有用なものだと思いますので、面接官をしない方にも読んでもらいたいです。  
なお内容としては「これを避けたい」がメインです。  

私の判断基準は「チームで一緒に働けると感じるかどうか、エンジニアの常識をある程度持っているか」だからです。  
基本的に優秀な方を採用したいのですが、本当に優秀かどうかを見抜くのは非常に難しいです。  
普通に話していてもどういった技術を知っていてそれに精通しているかはわかりません。  
そのため会話の中で違和感がないかを探り採用しない方を決める方向になります。

主にSystem Design Interview系のやり方を採用しています。  
範囲広めの質問から始めて、これまで行なってきた仕事についての理解度や技術力を確認します。  
面接全体としては、チームメンバーとして一緒に働けるかどうかを見ます。  

まず、私の思う採用判断基準と面接官をしてわかったことについてまとめます。  
その後、具体的な面接方法やわかったことをまとめます。  
長いですが、どうぞお付き合いください。  

[目次]

- [面接官のコツというか感じたこととか](#面接官のコツというか感じたこととか)
  - [更新日](#更新日)
  - [私が面接を行う際の採用可否判断基準](#私が面接を行う際の採用可否判断基準)
  - [応募者の振る舞いで気付いた、できれば避けてほしいこと](#応募者の振る舞いで気付いたできれば避けてほしいこと)
    - [応募者の一定数は、そもそも質問に正しく回答できず会話がうまくいかない](#応募者の一定数はそもそも質問に正しく回答できず会話がうまくいかない)
    - [応募者の一定数は、自分が行ってきた作業が全体のどこに位置して何故その方式で作るのかを理解していない](#応募者の一定数は自分が行ってきた作業が全体のどこに位置して何故その方式で作るのかを理解していない)
    - [応募者の一定数は、自分がこれまで使ってきたプログラミング言語の特性の違いを理解していない](#応募者の一定数は自分がこれまで使ってきたプログラミング言語の特性の違いを理解していない)
    - [応募者の一定数は、分からないことを分からないと言えない](#応募者の一定数は分からないことを分からないと言えない)
    - [応募者の一定数は、最近学習している技術的な内容の具体的詳細について答えられない](#応募者の一定数は最近学習している技術的な内容の具体的詳細について答えられない)
    - [新卒採用の応募者の一定数は、自身が行っている研究内容や専攻内容の詳細を答えることができない](#新卒採用の応募者の一定数は自身が行っている研究内容や専攻内容の詳細を答えることができない)
    - [ジュニアクラスの応募者は、詳しく説明しようとしすぎて不要なことを話しすぎる傾向にある](#ジュニアクラスの応募者は詳しく説明しようとしすぎて不要なことを話しすぎる傾向にある)
    - [ジュニアクラスの応募者は、誤りや不足を指摘された時にネガティブな返答をしてしまいそこで話が途切れる傾向にある](#ジュニアクラスの応募者は誤りや不足を指摘された時にネガティブな返答をしてしまいそこで話が途切れる傾向にある)
    - [マネージャーロールでの応募者の一定数は、システムについて全く理解していない](#マネージャーロールでの応募者の一定数はシステムについて全く理解していない)
    - [マネージャーロールでの応募者の一定数は、開発プロセスで行うべき手順及びその中身について答えられない](#マネージャーロールでの応募者の一定数は開発プロセスで行うべき手順及びその中身について答えられない)
    - [応募者の一定数は、やりたいことができない存在しないロールを想定して応募してくる](#応募者の一定数はやりたいことができない存在しないロールを想定して応募してくる)
  - [具体的な面接内容について](#具体的な面接内容について)
    - [前提](#前提)
      - [一般的な面接](#一般的な面接)
        - [アイスブレイクと自己紹介と会社のこと](#アイスブレイクと自己紹介と会社のこと)
        - [直近の仕事内容と経歴で気になった内容](#直近の仕事内容と経歴で気になった内容)
      - [行動面接](#行動面接)
      - [コーディング面接](#コーディング面接)
      - [SystemDesign系面接](#systemdesign系面接)

## 私が面接を行う際の採用可否判断基準

判断基準は「チームで一緒に働けると感じるかどうか」です。  
『チームに居たら困る方を採用しないこと』を重要視しています。  

以下の内容をどんどん掘り下げて聞いていきます。  
私の基準の場合、これだけでほぼ全ての応募者の採用判断が可能です。  

これらを理解している方は入社後に新しく使用する技術なども問題なく習得できるだろうと踏んでいます。  
カルチャーマッチなども重要ですが以下で気になる所がない場合のみ考慮しています。

- 担当部分はどういう構成か
  - なぜその構成を採用するのか
- 担当部分だけでなく全体はどういう構成か
  - なぜその構成が選ばれたのか
- 使う技術/ツールはどういう性質を持つか
  - なぜその技術/ツールを選ぶのか

中途採用の場合は過去の仕事を聞くことが多いです。  

過去の仕事内容が技術的に深掘りしようが無い場合は[SystemDesign系面接](#systemdesign系面接)課題で技術力を判断します。  
日本特有かもしれないですが、多重下請け構造でエンジニアをされている方の応募が多くあります。  
こういった方の仕事内容はほとんど作業のみとなっている場合があり、過去の経験から技術力が判断できない場合があります。  
しかし、これは日本社会のせいであって応募者のせいではないので、差し引いて判断して面接を行うようにしています。  
応募者はレジュメスクリーニングを突破しており、過去の仕事内容は私が行う面接の判断に直接関係がないと考えです。

## 応募者の振る舞いで気付いた、できれば避けてほしいこと

面接をする中での応募者の振る舞い（できれば避けて欲しいこと）を羅列していきます。  
※ 私が「採用基準に満たない方を採用しないこと」を最重要視している都合上、ネガティブな話ばかりになります。  

### 応募者の一定数は、そもそも質問に正しく回答できず会話がうまくいかない

1. 応募者「xxを実装しました」、私「具体的にどういう手法を用いて実装しましたか？」
   1. 応募者「xxという機能があって、△△というデータが入ってきて、それを⚪︎⚪︎に変換する仕組みです」と機能の詳細を答える
      1. 機能の詳細については聞いてない、具体的な実装方式を聞きたいと質問している
         1. 一応「機能の説明ではなくて例えば、APIとDBでどうとか具体的なアーキテクチャや実装はどうしましたか？」とか聞き返しますが、これまでと同じ答えが返ってくることもしばしば発生する
         2. 「xx機能はDBからデータを取得するAPIで、Python使ってレイヤードアーキテクチャで実装しました」とか返してほしい
         3. ↑のように帰ってくると「そのAPIはどういうものですか？」や「なぜレイヤードアーキテクチャで実装しましたか？」などと質問しやすい
      1. あるいは「この質問は機能についてですか？それともアーキテクチャについてですか？細かい実装の作りですか？」などを逆に質問してほしい
         1. 一度や二度言い直したり聞き返したりすることを問題にはしません
            1. とはいえ、何回も何回も同じようなことを聞かれるとこちらも構えます
         1. 覚えてきたことを読み上げられても特に何かを判断できるわけではないので、あえてフワッとしたOpen Questionで答え方を確定させないように聞くことが多いです
2. 応募者「xxが問題で処理が遅くなっていたのでDBにIndex張りました」、私「なぜそうしたのですか？」
   1. 応募者「xxが問題で遅かったので対応するカラム△△にIndex張って速度改善しました」と答える
      1. それは既に知っている、なぜIndexを張るという解決方法を選んだのか聞いている
          1. 分散処理したりDBをパーティションで分けたり、リアルタイム処理を諦めて夜間バッチ使ったりなど、状況次第でやり方は色々ある
          2. 採用理由がわからないとそのやり方しか知らないからそのやり方を採用したと判断せざるを得ない
      2. 「理由」を聞いているのに、「機能・過程・結果」を答える方は意外と多い

### 応募者の一定数は、自分が行ってきた作業が全体のどこに位置して何故その方式で作るのかを理解していない

1. 全体を見ていないので、どういう仕組みでシステム全体が動いているかを全く知らない
   1. 私「そのリポジトリ内では貴方が作られた機能以外にどういう機能が実装されていましたか？」 、応募者「自分の作成部分以外は知らない」などと答える
      1. 最悪担当外の実装詳細は知らなくてもいいが、どういう機能の一部を作っていて他機能との関連性がどうなのかくらいは知っていてほしい
      2. 応募者「私の作った機能は会員情報関連機能で、その他ポイント情報などが実装されていて、サービス全体のバックエンド機能が実装されています」みたいな返答が来ると嬉しい
   2. 私「そのシステムのインフラは何でできていますか？」、応募者「自分は機能を実装していたのでインフラは知らない」などと答える
      1. こちらも同じ。応募者「AWSのEC2で作ってます」くらいでも良い
         1. 自分の担当以外にも興味を持っていてほしい
         2. 必ずしもシステム全体を知る必要はないが、おおよそのアーキテクチャと自分が作る機能の周辺機能は知っていてほしい
2. 自分が作った部分であっても単に作っただけで、なぜその機能が必要か、なぜそのアーキテクチャが採用されたのか理解していない
   1. 応募者「xx機能API作りました」、私「その機能はどういう用途ですか」、応募者「自分はバックエンドを作ってるだけでフロントのことは知らない」などと答える
      1. どういう理由でその機能が必要なのか、どう使われるのかは知っていてほしい
      2. 「自分の範囲以外は知らない」とか言われると困る
      3. はっきり言って「正社員採用受けにきたんですよね？単発作業依頼の応募じゃないですよ？」と思ってしまう

### 応募者の一定数は、自分がこれまで使ってきたプログラミング言語の特性の違いを理解していない

1. 応募者「CとPython使ってました」、私「CとPythonにはそれぞれどういう特性がありますか？」と質問しても答えられない
   1. C言語を使っているのに、メモリ管理の話が一切でてこないと流石に心配になる
   2. Pythonを使っているのに「コンパイルできて早くていいですよね！」とかそれだけを言われると困る
      1. 今回の場合はC言語との差異も含めて聞いているので、C言語側の特性としてよく言われることを初手で言われると心配になる
      2. 別にPythonをコンパイルしようと思えばできるが、あまり一般的ではないのでそこの補足はして欲しい
2. 応募者「○○が得意です/○○が好きです」、私「○○には△△と◇◇がありますが違いはわかりますか？」と質問しても答えられない
   1. 内容にも依りますが、公式ドキュメントの目次にあるような事は少し話せるくらいに知って置いてほしい
   2. 得意や好きだと言うのは細かいことも質問してくれと言っているに等しいので、ハードルが上がることは自覚しておいてほしい
      1. 逆にちゃんと詳しい場合はプラス評価もしやすいので言ってもらえると嬉しい

### 応募者の一定数は、分からないことを分からないと言えない

1. 私「○○機能を実装した時のアーキテクチャや実装方式を教えてください」、応募者「○○機能はxxデータを管理するもので、APIを使ってa,b,c項目をDBから取得します。DBは○○テーブルがあって、△△テーブルとJOINしてデータを取得します。それをSwaggerで決めた形式に整形して...」と延々と機能の処理フローを語る
   1. 具体的な機能の中身ではなくアーキテクチャや実装方式が知りたいです
   2. 「○○機能はAPIでDBに情報を読み書きします、またAPIの実装はNode.jsでトランザクションスクリプトで書いてます。またDBはリードレプリカを採用して負荷分散しています。」くらいが返ってきてほしい
      1. もちろん私からも「システムの構成全体を簡潔に表すためのアーキテクチャ図とかってありました？」などと聞き返すが、意味が分からない場合に同じ回答を連発される場合がある
   3. 分からないなら分からないでと言ってほしい
      1. 分からずに適当に設計実装される方が後々問題になるので、わからない場合はわからないと解答してもらえることを期待している
      2. あまりにも基本的なことを知らない場合は困るが、似たようなものを知ってたらそれを話すなどをしてもらえると嬉しい
         1. 「RDBはわかるけどKey Value Storeはあまり分からない」とかは経験上はありえる
      3. 知っていてほしいものは多いが、よく使われる方式を知っていれば十分だと思っている
         1. 知らなくても少し説明して理解が出来るなら働く上では問題ないと判断できるので、関連知識があることはできれば見せてほしい

### 応募者の一定数は、最近学習している技術的な内容の具体的詳細について答えられない

1. 私「最近興味のある技術分野はありますか」、応募者「⚪︎⚪︎に興味があり学習しています」、私「⚪︎⚪︎について具体的に教えてください」に対し答えられない
   1. 興味があることや学習しているものがあること自体は素晴らしいが、面接で聞いているのでそれなりに深掘りはします
   2. 文脈次第ですが、ツールを使って少し触っただけのものなどは話題に出さない方が良いです
      1. というのも「『面接の場』で⚪︎⚪︎に興味があると言っていた割には詳しくなかった」という事実だけが残るからです

### 新卒採用の応募者の一定数は、自身が行っている研究内容や専攻内容の詳細を答えることができない

1. 研究内容を質問された際の対策が不十分な応募者が多い
   1. 応募者「ロボット作ってました」
      1. 姿勢制御のことは聞きたくなる
   2. 応募者「Deep Learning系の機械学習してました」
      1. ニューラルネットワークのことは聞きたくなる
   3. 応募者「数学系出身でxx研究していました」
      1. (直接の研究内容はともかく)大学教養レベルの微積と線形代数は大体知っているものとして質問したくなります
   4. こういった「一定確率で聞かれてしかもその研究をしているのであれば当然答えられるべきこと」については準備しておいてほしい
      1. 全てに即答して欲しいわけでは勿論ないが、知っている人としての反応は期待している

### ジュニアクラスの応募者は、詳しく説明しようとしすぎて不要なことを話しすぎる傾向にある

1. 応募者「xxプロジェクトで⚪︎⚪︎機能を作りました」 、私「それはどういう機能ですか？」
   1. 応募者「⚪︎⚪︎機能は⚪︎⚪︎データが入ってきてそれを△△に変換するために××を使っていて、そして変換したデータを・・・」みたく長い
      1. 理解してもらいたい気持ちはわかるが、構造化して簡潔に話をしてほしい
      2. 面接官はそれなりに知識経験がある人がおこなうので「⚪︎⚪︎機能」と聞いた段階でおおよそのアーキテクチャを想像できている場合が多い
         1. 一般的なものは簡単に、特殊な部分は少し詳細に話をしてほしい
         2. 自己紹介をしているので、相手がどの程度システムに詳しい人なのかは考えて話をしてほしい
         3. 友達にスマホアプリを薦める時と祖父母に薦める時で同じ説明の仕方はしないはず

### ジュニアクラスの応募者は、誤りや不足を指摘された時にネガティブな返答をしてしまいそこで話が途切れる傾向にある

1. 応募者「xx作りました」私「⚪︎⚪︎について考慮していましたか？」
   1. 応募者「⚪︎⚪︎は考慮できていなかったです・・・」ここで沈黙する
      1. 考慮不足があるのは事実だが、それについて責めているわけではない
      2. 応募者「⚪︎⚪︎は考慮できていなかったです、もし⚪︎⚪︎を考慮するなら××処理を実装して担保します」とか返ってきてほしい
         1. もちろんこちらから「⚪︎⚪︎を考慮するなら、どういう風に設計実装変更しますか？」などは聞き返します
            1. そこで答えてもらえればそれで良いと思っています
         2. とはいえ「あーそこは××入れないとダメですねー」くらいは初手で返ってきてほしい
         3. 普段チームで会話して抜けやバグを見つけても作った人を怒ったりはしない、必要なのは改善策を決めて実行することでそのシミュレーションがしたい

### マネージャーロールでの応募者の一定数は、システムについて全く理解していない

1. 直近のプロジェクトでどういう言語でどういうアーキテクチャを採用していたのか答えられない
   1. 私がエンジニアリングマネージャーを想定しているのもありますが、WBS引いて工数管理するだけなら誰でもできる
   2. エンジニアリングマネージャーを想定しているので、アーキテクトに近い視座を持ってプロジェクト全体を把握してほしい
2. オフショア開発などで開発それ自体を委任しており何を作っているのかを答えられない
   1. 特にSIerの方などで工数管理に終始しており開発の現場を知らない方が多い印象

### マネージャーロールでの応募者の一定数は、開発プロセスで行うべき手順及びその中身について答えられない

1. もちろん開発方式によりプロセスは異なるが、最低限以下の工程が想像されることくらいはわかっていてほしい
   1. (アイデア出し→)市場調査→要件決め→方式検討→設計→インフラ構築→機能実装→テスト→リリース

### 応募者の一定数は、やりたいことができない存在しないロールを想定して応募してくる

論外。  
なぜかたまに居ますが、エージェントの方に話を聞くか募集要項を読むか人事の方に相談してもらうかするとミスマッチが防げます。  

## 具体的な面接内容について

まず前提の共有です。

### 前提

- 想定ロール
  - エンジニア(ジュニア〜シニア、アーキテクトレベル)
  - マネージャー(エンジニアリングマネージャー)
- 面接形式
  - 一般的な面接
  - 行動面接
  - コーディング面接
  - SystemDesign系面接

#### 一般的な面接

いわゆる特別な対策を必要としない面接です。  
私が面接官の場合は以下の流れで進めています。  
基本的に仕事内容を聞いていく中で[SystemDesign系面接](#systemdesign系面接)のような質問をします。（エンジニア、マネージャー問わず）  

- アイスブレイク
- 会社のこと
- 自己紹介
- 経歴の中で直近の仕事内容
- その他の経歴で気になった内容
- 必要があれば[SystemDesign系面接](#systemdesign系面接)っぽい課題議論
- 採用条件とか諸々
- 逆質問コーナー

##### アイスブレイクと自己紹介と会社のこと

単に会話をして自社のイメージなどを聞いています。  
自己紹介では主に、会社での役割とプロジェクトでの役割を私は話します。  
応募者には好きに自己紹介してもらいますが、少なくとも直近の仕事あるいは最近自主的に取り組んでいる新しい技術などは話していただくようにしています。  

##### 直近の仕事内容と経歴で気になった内容

そのプロジェクト内での具体的な仕事とロールを確認します。  
はじめは弊社採用時の希望ロールは聞かずにここでの話ぶりから自社で適当なロールを想像しながら質問内容を考えます。  

実際に担当していたプロジェクトについて、[SystemDesign系面接](#systemdesign系面接)のような質問を行なっていきます。  

#### 行動面接

自社の求める人材としての振る舞いができるかを確認します。  
「チームでxxが起きました、その場合はどうしますか？」みたいな質問をします。  
基本的にはチームで課題解決ができるか、適切なコミュニケーションがとれるかを見ています。  

#### コーディング面接

基本的にはしないですが、場合によってはコーディング面接に近いことを口頭でします。  
TBD ...

#### SystemDesign系面接

徐々に深掘りして応募者の想定範囲から出るように質問していきます。  
いきなり課題をだすよりは過去に経験された仕事内容をもとにSystemDesignっぽい質問をしながら面接を進めるすることが多いです。  

わかっている人は設計実装細部、また使用しているフレームワークや言語の特性まで答えられます。  
わかっていない人は実際に具体作業としてやったことそれ単体の内容しか答えられないです。  
新卒の場合はやや話が変わりますが、ガクチカなどやってきたことについて同様に色々聞きます。

(※ 問題例 : ⚪︎⚪︎さんが開発されたシステム全体のアーキテクチャとその具体的な実装方式やフレームワークについて教えてください)  
(※ 問題例 : ブラウザにURLを入力して、画面が表示されるまでに何が起きていますか？)  

- 例① エンジニア
  - 応募者「Twitterのホーム画面作ってました」、私「どういったアーキテクチャですか？」
  - ここの返事で大体のレベルが分かります
    - A : 応募者「UIはReactで、バックエンドはマイクロサービスAPIで作っています」
      - **まだどのくらい理解しているかはわからないが「中身掘っていけばどれくらいの理解度かわかるかな？」と思う**
        - どうしてその構成を採用したのか質問したくなります  
        - フロントの話題がでた時点で、フロントエンドファイル構成の詳細やAPI連携周りを質問したくなります
        - マイクロサービスというワードが出ると、負荷分散やデータ整合性、セキュリティやセッション管理などを聴きたくなる
      - **本来あるべきな設計アーキテクチャから少し外した質問をするとどう返答するかも気になる**
        - 私「マイクロサービスというと、障害に強く基本的にはエラーで止まらないことがメリットでしたっけ？」のような質問をする
          - これは極端だが「そうですね！マイクロサービスは常に安定稼働するので安心です！」とか言われると困る
          - 応募者「いえ、単一障害点が発生しうるので、冗長性を確保する必要はありますね。例えばAPI部分は複数サーバ用意してロードバランサー入れてます」みたいな返答がほしい
        - 本来こういった質問をチーム内で行うことはまずないが、理解度を試すためにはどうしても不自然な質問をする場合はある
          - 面接官は絶対ではないし単に誤って覚えていることもあるので、それに対する指摘はしてほしい
          - 同僚と一緒に仕事するときに誤りを指摘できないのは困る

TBD...
