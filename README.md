# C++の基本
## 0日目
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
1. `using namespace std;`は指定された名前(今回はstd)の名前空間を使うことを意味している。4行目のcoutはここに定義が含まれている。
1.  `int main(){......`は
