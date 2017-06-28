# SKEye-Unity-SDK
SKEye-Unity-SDK for Object Recognition Service 
###  更新日志
v1.0.2
- 优化网络模块请求

v1.0.1
- 增加图像偏色处理接口（调整图像偏色：偏红、偏绿、偏蓝）
  
  备注：如需使用该接口，请在SDK初始化后调用一次即可。如果图像不需要偏色处理，则不需要调用该接口。

v1.0.0
- 发布常见物体识别、水果识别功能
###  目录介绍
- SKEye-Unity-SDK.unitypackage: unity包。
- 说明文档 [《SKEye-Unity-SDK说明文档v1.0.2.pdf》](https://github.com/interjoy/SKEye-Unity-SDK/blob/master/SKEye-Unity-SDK%E8%AF%B4%E6%98%8E%E6%96%87%E6%A1%A3V1.0.2.pdf)
###  使用步骤
- 下载SKEye-Unity-SDK.unitypackage文件包。
- 将SKEye-Unity-SDK.unitypackage导入Unity。
- 打开WebCamera场景，配置好申请的Api Key和Api Secret。
- 运行代码。
- 更多使用介绍请参考 [《SKEye-Unity-SDK说明文档v1.0.2.pdf》](https://github.com/interjoy/SKEye-Unity-SDK/blob/master/SKEye-Unity-SDK%E8%AF%B4%E6%98%8E%E6%96%87%E6%A1%A3V1.0.2.pdf)。
###  调用示例
    void Start () {
        PluginImportManage.Instance.MouseOver += Listener;

    }

    //调用接口
    void PSRecClick()
    {
        Flag = true;
        PluginImportManage.Instance.SKEyeSDKPhotograph();
        WebCameraImg.Instance.StopWebCamera();
    }

    void Listener(string _ResurtStr) {
        textResurt.text = _ResurtStr;

    }
###  SDK问题反馈
- SKEye开放平台QQ群：617518775
