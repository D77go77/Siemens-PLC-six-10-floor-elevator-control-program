
# Siemens PLC Elevator Control Program

## 项目概述

本项目包含了使用Siemens PLC（西门子可编程逻辑控制器）实现的一个6部10层电梯控制系统的示例程序。通过该程序，您可以了解如何用PLC逻辑和梯形图设计控制多个楼层的电梯运行。

## 功能特点

- **多楼层控制**：支持10层楼的电梯逻辑控制。  
- **楼层呼叫响应**：用户可以通过外部信号（如按钮）呼叫电梯到目标楼层。  
- **运行方向判断**：根据目标楼层与当前楼层的位置，决定电梯的运行方向。  
- **到站指示**：在电梯到达目标楼层时触发到站信号。  
- **超时保护**：加入运行超时逻辑，避免电梯长时间无响应。

## 文件说明

- `MainProgram.ld`：主程序梯形图文件，包含核心控制逻辑。  
- `FloorCallLogic.ld`：楼层呼叫处理逻辑的子程序。  
- `DirectionControl.ld`：电梯运行方向判断逻辑。  
- `ProtectionLogic.ld`：超时保护逻辑模块。

## 运行环境

- **PLC型号**：Siemens S7-1200 或以上版本  
- **编程软件**：TIA Portal V18 及以上版本  
- **硬件要求**：支持10个数字输入（楼层呼叫信号）和若干数字输出（电梯方向和到站信号）

## 使用说明

1. 将项目文件导入到TIA Portal中。  
2. 确保PLC硬件与程序中的输入/输出地址对应。  
3. 编译并下载程序到PLC设备中。  
4. 通过实际的楼层呼叫信号测试电梯的运行状态。  
5. 根据测试结果，调整参数或优化逻辑。

## 贡献

欢迎提出问题、提交功能需求或改进建议。  
您可以通过[创建Issues](https://github.com/D77go77/Siemens-PLC-six-10-floor-elevator-control-program/issues)的方式与我们沟通。

