## ファクトリ
各操作はアトミックであるべき。

- 値オブジェクトファクトリ
完全な状態で生成される。
- エンティティファクトリ
有効な集約を生成するのに必要な、本質的な属性だけを受けとるようにする。
　→それ以外ならば、後から追加できるようにすれば良い。
新しい追跡IDを割り当てることがない。
