# MO-DBPC-LLM-Agent: 电机控制算法推导与仿真辅助大模型智能体

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Topic](https://img.shields.io/badge/Domain-Power_Electronics_&_Motor_Drives-success)
![Status](https://img.shields.io/badge/Status-Active_Development-orange)

## 📌 项目简介 (Introduction)
本项目旨在构建一个垂直领域的 AI Agent，专门用于解决电力电子与电气传动领域（特别是三电平 NPC 逆变器与 PMSM 驱动）中，复杂控制算法的数学推导与代码生成问题。
当前核心落地场景为：**复合多目标无差拍控制策略（MO-DBPC）的解析寻优与 Simulink 闭环仿真加速**。

## ⚙️ 核心功能 (Core Features)
- **长链微积分推导**：自动化处理包含中点电压偏差与占空比平滑项的二次型代价函数，基于拉格朗日极值定理导出最优分配因子的代数解析解。
- **跨模态代码编译**：将纯数学理论推导（LaTeX）自动向下转化为 MATLAB `.m` 脚本与 Simulink C-MEX S-Function 底层发波代码。
- **论文级图表排版**：根据工程仿真数据，自动化生成符合 IEEE 期刊规范的实验数据对比图表。

## 🚀 应用场景 (Use Cases)
- 20kW 级高动态牵引电机控制算法研发。
- 突加满载极限工况（如 40N·m 阶跃）下的抗扰鲁棒性闭环验证。
- 降低传统 FCS-MPC 在线遍历寻优带来的微处理器“算力爆炸”问题。

## 🔒 声明 (Disclaimer)
由于本项目涉及部分商业级仿真订单代码以及未发表的学术毕业论文核心算法，当前 GitHub 仓库仅展示架构逻辑与 Agent 交互规范，核心源码暂不开源。