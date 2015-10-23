#C++11

##概要
C++11とは、2011年8月に改訂され、ISO/IEC 14882:2011で標準規格化されたC++バージョンの通称である。

前バージョンであるC++03からメジャーバージョンアップされ、多くの有用な機能が追加された。

このバージョンは、策定中はC++0xと呼ばれていた。これは、2009年中までに策定を完了させることを目指して、下一桁を伏せ時にしたものである。


##言語機能

| 言語機能       | 説明 |
|----------------|------|
| `alignas`      | アラインメント指定 |
| `alignof`      | アラインメント取得 |
| `auto`         | 型推論 |
| `decltype`     | 式の型を取得 |
| 定義済みマクロ | C++11で更新された定義済みマクロ |
| `constexpr`    | 定数式 |
| 関数の`default`／`delete`宣言 | 自動定義される特殊関数の制御 |
| 移譲コンストラクタ      | コンストラクタから他のコンストラクタに処理を移譲する |
| `explicit operator T()` | 明示的型変換の演算子オーバーロード |
| 拡張`friend`宣言        | テンプレートパラメータや`typedef`名を`friend`宣言する |
| `extern template`       | テンプレートのインスタンス化を抑止する |
| 継承コンストラクタ      | 基本クラスのコンストラクタを継承する |
| ラムダ式                | 関数オブジェクトをその場に書く |
| ローカルクラスと無名クラスを、テンプレート引数として使用する | |
| インライン名前空間      | ネストした名前空間に、透過的にアクセスする |
| `char16_t`、`char32_t`  | UTF-16とUTF-8の文字型 |
| Unicode文字列リテラル   | UTF-8、UTF-16、UTF-32のエンコーディングを規定したプレフィックス |
| 生文字列リテラル        | エスケープシーケンスを無視する |
| ユーザー定義リテラル    | リテラルのサフィックスをユーザー定義する |
| 戻り値の型を後置する関数宣言構文 | 戻り値の型を後ろに書けるようにすることで、パラメータオブジェクトを戻り値型の文脈で使用できるようにする |
| [`nullptr`](cpp11/nullptr.md) | ヌルポインタを表すポインタリテラル |
| テンプレートの右山カッコ | `vector<basic_string<char>>`のように、`>>`をスペースを空けずに記述可能にする |
| 右辺値参照・ムーブセマンティクス | 右辺値によるオーバーロード、およびそれによるリソースの所有権移動 |
| `static_assert`  | コンパイル時アサート |
| `enum`の先行宣言 | `enum`の先行宣言を許可する |
| `enum class`     | 強い型付けとスコープを持つ列挙型 |
| エイリアステンプレート | テンプレートによって型の別名を定義する |
| `union`の制限解除 | 共用体のメンバ変数として、クラスオブジェクトを持てるようにする |
| 可変引数テンプレート | 任意の数のテンプレートパラメータを受け取れるようにする |
| 範囲for文 | 配列やコンテナといった範囲を表すオブジェクトを、簡潔に走査する |
| `override`と`final` | メンバ関数のオーバーライド指定、および派生クラスでのオーバーロードの禁止を指定する |
| 属性構文 | `[[attr]]`構文による、クラス、関数、変数の属性指定 |
| メンバ関数の左辺値／右辺値修飾 | オブジェクトが左辺値／右辺値の場合のみ呼び出し可能であることの指定 |
| 非静的データメンバの初期化 | メンバ変数を、宣言と同時に初期値指定する |
| 初期化子リスト | 波括弧による初期化をユーザー定義する。`vector<int> v = {1, 2, 3};`など。 |
| 一様初期化     | コンストラクタの呼び出しを、波カッコで行う。`T x {a, b, c};` |
| `noexcept` | 関数の例外指定、例外を投げる可能性のある式か`boolP値を返す演算子 |
| 任意の式によるSFINAE | 特定の式が有効かどうかで、その関数をオーバーロード解決に含めるかどうかを決定する |
| `thread_local` | スレッドローカルストレージ |
| ブロックスコープを持つ`static`変数初期化のスレッドセーフ化 | |


###C99互換機能

| 言語機能       | 説明 |
|----------------|------|
| 可変引数マクロ | マクロで任意の数の引数を受け取る |
| `_Pragma`      | 処理系定義の機能を使用する単項演算子 |
| 定義済みマクロ | C99互換で導入された定義済みマクロ |
| 文字列リテラルとワイド文字列リテラルの結合 | ワイド文字列定数として結合する |
| `long long`型 | `long`以上の大きさを持つ整数型 |


##参照
- [C++11 Overview - Standard C++](https://isocpp.org/wiki/faq/cpp11)
