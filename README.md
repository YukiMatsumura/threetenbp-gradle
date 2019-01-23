# threetenbp-gradle

  

[ThreeTen backport project](https://github.com/ThreeTen/threetenbp)の`TzdbZoneRulesCompiler`を使ってTZDB.datを作るGradle.

  

```
手順1. プロジェクトルートに`/tzdb`フォルダを作成
mkdir tzdb

手順2. TZDBを解凍して配置（フォルダ名は `[12][0-9][0-9][0-9][A-Za-z0-9._-]+` にマッチすること）
mv {tzdb}/2018i {threetenbp-gradle-root}/tzdb/2018i

手順3. gradle実行
./gradlew tzdb

手順4. `/build/tzdb`に`TZDB.dat`が出力されていることを確認
cat {threetenbp-gradle-root}/build/tzdb/2018i
```

