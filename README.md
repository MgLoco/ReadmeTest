csv.h
====
センサ出力(CSVファイル)のROW×COLのデータを扱うためのライブラリ

## マクロ定義
---
CSVファイルは、データを取得する際に指定した行数と列数で構成される。ここでは行数と列数ともに60で固定のものとして扱うようにした。

| Name | Value | Content |
|:----:|:-----:|:-------:|
| ROW  | 60    | CSVファイルの行数 |
| COL  | 60    | CSVファイルの列数 |

## void clearData(int data[ROW][COL])
---
データ配列を0でクリアする。

### 引数
* data[ROW][COL] ... ROW×COLのデータ配列

## void dispData(int data[ROW][COL])
---
データを表示する。

### 引数
* data[ROW][COL] ... ROW×COLのデータ配列

## void copyData(int src[ROW][COL], int dst[ROW][COL])
---
データをコピーする。

### 引数
* src[ROW][COL] ... コピー元データ配列
* dst[ROW][COL] ... コピー先データ配列

## void readData(char \*fname, int data[ROW][COL])
---
CSVファイルからデータを読み取り、データ配列に格納する。

### 引数
* \*fname ... CSVファイル名
* data[ROW][COL] ... ROW×COLのデータ配列

## void writeData(char \*fname, int data[ROW][COL])
---
CSVファイルにデータを書き込む。

### 引数
* \*fname ... CSVファイル名
* data[ROW][COL] ... ROW×COLのデータ配列

## void addData(int a[ROW][COL], int b[ROW][COL], int c[ROW][COL])
---
2つのデータ配列を加算する。

### 引数
* a[ROW][COL] ... 加算を行う1つ目のデータ配列
* b[ROW][COL] ... 加算を行う2つ目のデータ配列
* c[ROW][COL] ... 加算結果を格納するデータ配列

## int getMaxDatum(int data[ROW][COL])
---
データの最大値を取得する。

### 引数
* data[ROW][COL] ... 対象となるデータ配列

### 戻り値
* max ... データ最大値
