# glibc-gconv-extra lambda layer

AWS Lambda runtimes for Python 3.12 and later are based on Amazon Linux 2023, which does not include the glibc-gconv-extra package by default. As a result, using ODBC connections may cause “Unicode conversion failed (22) (SQLGetData)” errors. This Lambda layer provides the necessary components to resolve this issue.

> [!IMPORTANT]
> Remember to set the Lambda environment variable GCONV_PATH=/opt/lib/gconv

