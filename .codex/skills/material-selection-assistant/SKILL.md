<!-- 固定工作流约束：本文件属于05 材料与氛围设计，不得改变九模块架构及执行顺序。 -->

> **模块归属：05 材料与氛围设计**
>
> **全局流程：01 → 02 → 03（概念方案汇报与客户确认）→ 04 → 05 → 06 → 07 → 03（完整设计汇报与客户确认）→ 08 → 09。**
>
> 本模块只在对应阶段执行。第一次 03 未取得客户明确确认，不得进入 04；第二次 03 未取得客户明确确认，不得进入 08。任何修改应返回对应模块，更新版本后重新汇报。不得新增、拆分或重新编号模块。具体职责与确认规则以 `.codex/skills/COMMON_RULES.md` 及总控 Skill 为准。

---

---
name: material-selection-assistant
description: Analyze and recommend interior design materials based on design concepts, spatial functions, atmosphere goals, durability requirements, maintenance needs, and budget considerations.
---

# Material Selection Assistant / 材料选择助手

## Purpose / 目的

Select appropriate interior materials that support design concepts, spatial functions, user needs, atmosphere, durability, and budget.

根据设计概念、空间功能、用户需求、氛围目标、耐久性和预算选择合适的室内材料。

---

## Basic Rules / 基本规则

1. Analyze the design concept and translate it into material language.

分析设计概念，并转化为材料语言。

2. Recommend materials according to space function and user requirements.

根据空间功能和用户需求推荐材料。

3. Consider appearance, texture, durability, maintenance, and cost.

综合考虑视觉效果、质感、耐久性、维护和成本。

4. Establish material combinations including flooring, walls, ceiling, furniture, and decorative elements.

建立完整材料组合，包括地面、墙面、顶面、家具和装饰元素。

5. Provide alternatives for different budget levels.

根据不同预算提供替代方案。

---

## Output Format / 输出格式

1. Design Concept Understanding / 设计概念理解

2. Material Strategy / 材料策略

3. Flooring Recommendation / 地面材料建议

4. Wall & Ceiling Materials / 墙顶材料建议

5. Furniture & Soft Material Direction / 家具软装方向

6. Color & Texture Palette / 色彩与质感

7. Budget Alternatives / 预算替代方案

8. Maintenance Considerations / 维护建议

9. Further Questions / 深化问题

## 共同规则（必须遵守）

开始执行本技能前，必须读取并遵守共同规则文件：`.codex/skills/COMMON_RULES.md`（相对于本技能目录的路径为 `../COMMON_RULES.md`）。该文件中的工作前思考、底图与几何锁定、简洁优先、精准修改及结果验证要求，均适用于本技能。

如果无法读取共同规则文件，不得声称已读取或已遵守；应明确说明，并优先保护原始底图、尺寸、比例和用户明确指定的限制。


## 05 材料与氛围设计（整合专业子项）

本模块统一完成材料、灯光和软装设计，三个专业方向在同一份设计成果中协同，不再拆成三个独立工作流。

### 材料
- 根据设计概念、空间功能和预算确定地面、墙面、顶面、家具及装饰材料。
- 综合考虑颜色、质感、耐久性、维护方式、环保要求和成本。
- 输出材料策略、色彩与质感板、材料清单、品牌型号及预算替代方案。

### 灯光
- 建立基础照明、功能照明、重点照明和装饰照明层次。
- 协调空间功能、材料反射、视觉舒适度、色温和能耗。
- 输出灯光策略、灯具方向、色温氛围、控制建议及预算选项。

### 软装
- 根据已确认的概念和空间布局，完成家具、织物、地毯、窗帘、艺术品、装饰品及植物陈设方向。
- 考虑人体尺度、生活习惯、舒适度、收纳需求和空间比例。
- 输出家具清单、软装搭配、色彩组合、织物策略、艺术陈设及生活场景建议。

### 05 统一交付
材料表、灯光策略、软装清单、色彩与氛围板、预算替代项及提供给 07 的可视化说明。所有内容必须遵循 02 的概念方向和 04 的已确认空间规划，不得改变固定布局或建筑结构。
