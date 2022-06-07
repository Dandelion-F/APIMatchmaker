# APIMatchmak

## 运行步骤

1. 使用 getSDKVersion.py 获取每个应用的 SDK 版本，包括最低版本（minSdkVersion）和目标版本（targetSdkVersion）。

2. 使用 PresolvedCSVFilter.py 处理应用描述。

3. 使用 lib/APIExtractor.jar 提取每个应用的方法声明和 API 调用。

4. 使用 DatasetGenerator.py 生成数据集的评估结果。

5. 运行 main.py 启动程序。其中的 **getOptions()** 函数有对参数进行详细说明。
    

## 代码结构

1. **lib** 目录包含了一个从 APK 文件提取方法和 API 的工具实现。

2. **Dataset** 目录提供了可访问该数据集的链接地址。

3. **Helper** 目录包含了一些基本功能实现，例如，收集应用描述的爬虫程序。

4. **Main** 目录包含了最核心的代码，包括推荐方法的实现。