# HuPhoneISP
ISP Demo

graph LR
    A[RAW图像输入] --> B(AI-ISP预处理)
    B --> C{动态引擎}
    C --> D[3A算法模拟]
    D --> E[HDR融合]
    E --> F[虚拟传感器输出]

    graph TD
    A[RAW图像] --> B(AI降噪)
    B --> C(AWB校正)
    C --> D(AE控制)
    D --> E(HDR融合)
    E --> F[JPEG输出]

Add param detail
技术栈：Python + OpenCV + PyTorch

数据集：MIT-Adobe FiveK4

关键指标：

PSNR > 30dB（vs 原厂ISP）

1080P处理延迟 < 15ms4
