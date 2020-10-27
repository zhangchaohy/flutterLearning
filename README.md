1、把文件拷贝到dart-sdk/bin/snapshots中

2、修改dart-sdk/bin/pub文件 用记事本打开

3 if defined USING_DART_1 (
  echo "Pub no longer supports Dart 1"
) else (
   rem "%BIN_DIR%\dart" %VM_OPTIONS% "%BIN_DIR%\snapshots\pub.dart.snapshot" %*修改为
  "%BIN_DIR%\dart" %VM_OPTIONS% "%BIN_DIR%\snapshots\my.pub.snapshot" %*
)

