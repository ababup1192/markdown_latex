# はじめに

これはテストです。書式はgithubのmarkdownを採用しています。


# いろいろな書式

## subsection的な

* 箇条書きも対応してほしい
* itemizeとか毎回書くのまじでしんどい
    * 入れ子とかもサポートしてくれると良いよね

### subsubsection的な

1. もちろん、数字のサポートも必須でしょ
    * 違うアイテマイズの入れ子ももちろんサポートするよね

# 画像

\begin{figure}[htb]
  \centering
  \includegraphics[width=3cm]{src/img/latex}
  \caption{画像}
\end{figure}


# 文字書式

* これはイタリック体です*
* _これもイタリック体です_
* これはイタリック体になりません
* **これは太字です**
* __これも太字です__

> 引用はどうなるんだろう

# 表はどうなる

|カラム1|カラム2|
|------|------|
|hoge|geho|
|age|sage|

# プログラム
	#incldue <stdio.h>

	int main(){
		printf("hello world\n");
	}
