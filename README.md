# C++の基本
## 0日目
### 基本要素について
C++のファイルは.cppファイル<br>
基本的に定義、宣言、出力の順番<br>
### オブジェクト指向とは
概念の大きさの順番:クラス＞オブジェクト（インスタンス）＞属性＝メソッド<br>
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
1. `using namespace std;`は指定された名前(今回はstd)の名前空間を使うことを意味している。4行目のcoutはここに定義が含まれている。Cでは同じ変数を使えなかったが、C++では名前空間が違うなら同じ変数を使ってもいいとする。
1.  `int main(){......`はintは最終的に整数を返すという意味、mainは最初に呼び出される関数のこと、()には引数が入る。引数と変数の違いは変数はその関数内のみ（今回ならint main()）の定義だが引数としint aなどを入れるとmain(2)などのプログラムはmain関数に2の値の結果が使われる。
1. ` cout << "HelloWorld." << endl` は関数ではないが、printf関数と同じ働き。実はオブジェクト。coutを通じてHelloWorld.を送り出している。endlは改行
1. `return ;`は関数の処理をそこで終わらせて、値を呼び出し元に返すという意味。`return　0;`はOSに正常に終了したことを伝える。`return　1;`はOSに正常に終了せずにエラーが起きたことを伝える。
1. `using namespace std;`と` cout << "HelloWorld." << endl;`を統合して`std::cout << "HelloWorld." << std::endl;`にできる。
1. 
