# 量潮数据云

本产品还处于寻找方向的早期阶段，随着对这一领域理解的增加，会不停地调整方向直到稳定。

## 原则

云和开源两条腿走路。

## 产品战略

计算功能可以考虑以下几个方案：

1. AirFlow。通用编排工具。初步感觉符合我们需求，且预计兼容性较好。
2. Beam及Google DataFlow。更主要关注机器学习计算，和Flink等计算引擎兼容性好。
3. 云厂商提供的函数计算工作流。已经被验证不好用的方案。
4. 容器编排方案。尽量不用容器，优先使用函数。
5. Flink。实时计算，暂时用不上。

关于AirFlow和Beam的对比：

- https://www.astronomer.io/blog/airflow-vs-apache-beam/
- https://stackoverflow.com/questions/50249759/apache-airflow-or-apache-beam-for-data-processing-and-job-scheduling

如果以Airflow为主体搭建：

1. 不动核心模块，在此基础上通过插件（AirFlow Plugin）拓展功能。
2. 二次开发Airflow的核心模块，如果确实无法满足我们需求。

主要计划拓展的特性是：

1. 腾讯云等国内云厂商，主要是云原生相关。
2. 企业微信等国内的企业账号，比如WebHook消息通知。


## 开源战略

1. 尽可能在AirFlow已有的生态上构建，以最大限度地利用开源社区提高产品质量。
2. 尽可能地回馈AirFlow社区，同时也形成开打闭的商业模式。


## 项目管理

- 第一个版本：部署Airflow，并且逐步看是否可以注册。
- 第一个里程碑：对数据分析任务使用，提高项目上云函数以后的运行效率。


## 品牌管理

由于AirFlow的开源协议是Apache 2.0，因此我们必须要带上AirFlow的名字宣传。有两种定位：

1. 量潮数算云。兼容或者部分兼容AirFlow的二次开发的自研平台。
2. 量潮AirFlow。AirFlow及其Plugin拓展的云端版本。
