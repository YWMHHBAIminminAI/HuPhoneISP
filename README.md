# HuPhoneISP
ISP Demo

graph LR
    A[RAW图像输入] --> B(AI-ISP预处理)
    B --> C{动态引擎}
    C --> D[3A算法模拟]
    D --> E[HDR融合]
    E --> F[虚拟传感器输出]
