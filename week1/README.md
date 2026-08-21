# DL-notes（深度学习学习记录）

> 目标：为大二下 LLM4EDA 论文做准备（LLM 生成 Verilog 质量评测方向）
> 主线并行：一生一芯（YSYX v24.07，当前 E 阶段）
> 环境：AutoDL（RTX 4090 / 无卡模式）+ PyTorch 2.8.0+cu128

## 本周（Week 1：2026.8.20–8.28）跑了什么

| # | 内容 | 状态 |
|---|---|---|
| 1 | 环境搭建 + 第一个张量（rand/shape/dtype） | ✅ 完成 |
| 2 | numpy 十连（reshape/切片/广播/轴统计）+ numpy↔tensor | ✅ |
| 3 | 自动微分：手算核对 4.5 梯度 + x² 求导 | ⬜ |
| 4 | 训练循环五步骨架（前向→loss→zero_grad→backward→step） | ⬜ |
| 5 | CIFAR-10 训练 1 epoch + 保存模型 | ⬜ |

## 验收清单（全部打勾才算过）

- [✔] AutoDL 能独立开/关实例，知道无卡模式和 4090 的切换
- [✔] 跑出第一个张量，看到 torch.Size([3, 4]) torch.float32
- [ ] numpy 十个常用操作不用查文档
- [ ] 能解释 4.5 的梯度怎么手算出来
- [ ] 能口述训练循环五步
- [ ] 仓库里有 3+ 个干净 notebook

## 问题清单（攒着，每周清）

- [ ] 为什么无卡模式下 nvidia-smi 存在但 /dev/nvidia* 没有设备？
