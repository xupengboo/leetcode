# LeetCode Algorithm Solutions

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/yourusername/leetcode/pulls)

多语言实现的LeetCode算法解析库，涵盖Python/Java/C++/Go/JavaScript等多种实现

## 📖 目录
- [项目特点](#-项目特点)
- [快速开始](#-快速开始)
- [目录结构](#-目录结构)
- [使用指南](#-使用指南)
- [贡献指南](#-贡献指南)
- [许可证](#-许可证)

## 🌟 项目特点
- **多语言实现** 每道题目提供至少2种语言实现
- **深度解析** 包含算法思路、复杂度分析和图形化示意图
- **分类索引** 按算法类型和难度等级双重分类
- **持续更新** 与LeetCode每周新题保持同步
- **测试驱动** 所有解法附带单元测试用例

## 🚀 快速开始
```bash
git clone https://github.com/yourusername/leetcode.git
cd leetcode/solutions/python
# 运行示例题解测试
python3 -m unittest 001_two_sum/test.py
```

## 📂 目录结构
```
leetcode/
├── solutions/               # 按语言分类的解决方案
│   ├── python/
│   │   └── 001_two_sum/     # 题目编号+名称
│   │       ├── solution.py  # 实现代码
│   │       ├── README.md     # 题目解析文档
│   │       └── test.py      # 单元测试
│   ├── java/
│   ├── cpp/
│   └── go/
├── docs/                    # 算法知识体系文档
│   ├── binary_search.md
│   ├── dynamic_programming.md
│   └── graph_theory.md
└── resources/               # 辅助学习资源
    ├── complexity.pdf       # 复杂度速查表
    └── cheat_sheet.png      # 算法思维导图
```

## 📝 使用指南

### 查找特定题目

```python
# 通过题号查找（推荐）
solutions/python/001_two_sum/README.md

# 通过算法类型查找
docs/dynamic_programming.md -> 相关题目列表
```

### 代码规范

- 变量命名使用LeetCode题目中的原始命名
- 每个解法必须包含时间/空间复杂度注释

```python
# Python示例
def two_sum(nums: List[int], target: int) -> List[int]:
    """
    时间复杂度：O(n)
    空间复杂度：O(n)
    使用哈希表实现一次遍历解法
    """
    num_map = {}
    for i, num in enumerate(nums):
        ...
```

## 🤝 贡献指南

欢迎通过以下方式参与贡献：

1. 提交新题解（请确保包含）
   - 至少两种语言实现
   - 解析文档（含示意图）
   - 边界测试用例
2. 优化现有解法
3. 补充算法理论文档

**代码提交规范**

- 目录命名：`{题号}_{题目名称}` (例：`015_3sum`)
- 文件命名：`solution.{语言后缀}`
- 提交信息格式：`[语言] 类型 题号` (例：`[Python] Add 015`)

## 📜 许可证

本项目采用 [MIT License](https://chat.deepseek.com/a/chat/s/LICENSE)

------

**相关资源**

- [LeetCode官网](https://leetcode.com/)
- [算法可视化网站](https://visualgo.net/)
- [复杂度速查表](https://chat.deepseek.com/a/chat/s/docs/complexity.pdf)

## 🛠 效果增强建议
1. 添加实际截图：
   ```markdown
   ![解题示意图](screenshots/demo.png)
   ```

2. 增加进度追踪表：

```markdown
## 📈 完成进度
| 分类 | 总题数 | 完成数 | 进度 |
|------|-------|-------|-----|
| 数组 | 150   | 120   | 80% |
| 树   | 80    | 65    | 81% |
```

3. 添加学习路线图：

```markdown
## 🗺 学习路线
​```mermaid
graph TD
  A[基础算法] --> B[排序与搜索]
  A --> C[递归回溯]
  B --> D[高级数据结构]
  C --> D
  D --> E[系统设计]
```

4. 增加自动化脚本提示：

```markdown
### 自动化工具
​```bash
# 生成目录索引（需要安装tree）
./scripts/generate_toc.sh
```