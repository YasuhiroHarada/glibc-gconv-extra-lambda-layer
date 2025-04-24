# glibc-gconv-extra lambda layer

The AWS Lambda runtime for Python 3.12 and later is based on Amazon Linux 2023, and the glibc-gconv-extra package is not included by default. Therefore, when using the Microsoft ODBC Driver with SQL_WCHAR, you may encounter an error such as "Unicode conversion failed (22) (SQLGetData)." This Lambda layer provides the necessary components to resolve this issue.

> [!IMPORTANT]
> Remember to set the Lambda environment variable GCONV_PATH=/opt/lib/gconv

Python 3.12以降のAWS LambdaランタイムはAmazon Linux 2023をベースにしており、glibc-gconv-extraパッケージがデフォルトで含まれていません。そのため、ODBC接続を使用すると「Unicode変換に失敗しました (22) (SQLGetData)」というエラーが発生する可能性があります。このLambdaレイヤーは、この問題を解決するために必要なコンポーネントを提供します。
 

