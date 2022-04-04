# interfaceとtypeの違い
```
let apple: { nickName: string; isHuman: boolean; level: number } = {
  nickName: "りんご",
  isHuman: true,
  level: 0
};
```
オブジェクトの型を定義するときに型アノテーションでやったら大変だし、読みづらいし、面倒くさい。。
<br></br>

## interface
```
interface Member {
  nickName: string;
  isHuman: boolean;
  level: number;
}

let apple: Member = {
  nickName: "りんご",
  isHuman: true,
  level: 0
};
```
TSではオブジェクトの型に名前をつけることができる。

## type
```
type Member = {
  nickName: string;
  isHuman: boolean;
　level: number;
};

let apple: Member = {
  nickName: "りんご",
  isHuman: true,
  level: 0
};
```
型に名前をつけられる方法としてはtypeというやつもあります。

