# 编译规则

本目录把 `source_prompt/` 编译为两种形态：

1. **standalone skill**：`opencode/` 下的装配说明；产物是单个 skill，可被任意 agent 触发。
2. **embedded module**：`嵌入说明.md`；作为更大认知工程的源域，参与宿主编译。

先读 `模块契约.md`，再按目标模式选路径：

- standalone：`opencode/装配说明.md` → `opencode/产物定义.md` → `opencode/验收.md`。
- embedded：`嵌入说明.md` → 宿主 `compile_prompt`。

不修改 `source_prompt/`；产物落在 `build/<platform>/` 下。
