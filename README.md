How to use the software:
您需要AndroidSDK来完成编译。此外，您必须有debian
下载此仓库文件并使用以下命令编译：
没有任何的程序.
CD ralseint

# 二选一：写死路径 或 用环境变量
echo"sdk.dir=/你的/Library/Android/sdk">local.properties
# export ANDROID_HOME=/你的/Android/sdk

./gradlew assembly调试#产物：app/build/outputs/apk/debug/app-debug.apk
./gradlew testDebugUnitTest      # 可选：跑那 15 条单元测试
adb install -r app/build/outputs/apk/debug/app-debug.apk

编译完成后，安装软件即可使用。
