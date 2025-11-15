# C++の基本
## 0日目
### 基本要素について
・C++のファイルは.cppファイル<br>
・基本的に定義、宣言、出力の順番<br>
・ストリームはデータ（数値や文字列など）を送り込んだり、逆に受け取ったりするもの。`cin`や、`cout`は、その流れからデータを受け取ったり、送り込んだりする。不等号の向きは、その流れの向きを表す。<br>
・`iostream`、`string`はヘッダというものでライブラリ。ライブラリはあらかじめダウンロードされている。
・`int main(){......`はintは最終的に整数を返すという意味、mainは最初に呼び出される関数のこと、()には引数が入る。引数と変数の違いは変数はその関数内のみ（今回ならint main()）の定義だが引数とし`int a`などを入れると`main(2)`などのプログラムはmain関数に2の値の結果が使われる。`return 0;`などでint mainのintに対して0を返している。
・`return ;`は関数の処理をそこで終わらせて、値を呼び出し元に返すという意味。`return　0;`はOSに正常に終了したことを伝える。`return　1;`はOSに正常に終了せずにエラーが起きたことを伝える。
### オブジェクト指向とは
・概念の大きさの順番:クラス＞オブジェクト（インスタンス）＞属性＝メソッド<br>
オブジェクト:プログラム上のモノ<br>
メソッド:オブジェクト(モノ）の動き<br>
属性:メソッドの情報そのもの<br>
## 1日目
```cpp
//Hello world(main.cpp)
#include <iostream>
 
using namespace std;
 
int main(){
    cout << "HelloWorld." << endl;
    return 0;
}
```
出力結果<br>
`HelloWorld.`

一行ずつ日本語に訳しながら説明する。<br>

1. `#include <iostream>`はiostreamというファイルを読み込むときに用いる宣言。単にヘッダと呼ばれる。
1. `using namespace std;`は指定された名前(今回はstd)の名前空間を使うことを意味している。cin、coutはここに定義が含まれている。Cでは同じ変数を使えなかったが、C++では名前空間が違うなら同じ変数を使ってもいいとする。
1.  `int main(){......`については上に示す。
1. ` cout << "HelloWorld." << endl` は関数ではないが、printf関数と同じ働き。実はオブジェクト。coutを通じてHelloWorld.を送り出している。endlは改行
1. `return 0;`については上に示す。
1. `using namespace std;`と` cout << "HelloWorld." << endl;`を統合して`std::cout << "HelloWorld." << std::endl;`にできる。
```cpp
//string
#include <iostream>
#include <string>
 
using namespace std;
 
int main(){
    string s,t;
    t ="入力された文字は、";
    cout << "文字列を入力：";
    cin >> s;
    cout << t+s << "です。" << endl;
    return 0;
}
```
出力結果
文字列を入力：Hello   ←キーボードから入力<br>
入力された文字は、Helloです。<br>

