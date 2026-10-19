# 英文生成提示词结构

参考展板用于上游分析。把分析结果完整写入提示词；生成时只绑定目标底图。下列占位项在生成前填写。

```text
Create a complete architectural presentation board using the attached building image
as the target project. This is a conceptual architectural communication study.
Output: [ORIENTATION, ASPECT RATIO, REQUESTED RESOLUTION].

TARGET BUILDING
Preserve [DISTINCTIVE MASSING, ROOF, OPENINGS, ENTRANCE, MATERIALS AND COLORS].
Maintain a coherent project identity across the main image, diagrams and supporting views.

BOARD COMPOSITION
[DESCRIBE THE REFERENCE LAYOUT IN FULL WITHOUT REQUIRING THE REFERENCE IMAGE:
COLUMN WIDTHS; REGION HEIGHTS; HERO; EXPLODED DIAGRAM; SIDE STRIPS;
LOWER BANDS; ALIGNMENTS; MARGINS; READING ORDER.]

CONTENT BY REGION
[REGION, DIAGRAM/VIEW TYPE, AND RELATIONSHIP TO THE TARGET BUILDING.]
Generate supporting axonometrics, conceptual plans/sections, diagrams and views
to populate the complete composition. Treat unknown spatial and structural details
as conceptual interpretations of the visible building, keeping internal consistency.
Do not substitute empty placeholders for diagram regions.

VISUAL LANGUAGE
[BACKGROUND, DIAGRAM PALETTE, LINE WEIGHTS, RENDERING, TYPE AND DENSITY.]

TEXT
Use [USER COPY OR DESCRIPTIVE TITLE AND CONCISE DIAGRAM LABELS].
Do not invent a real location, author, measured performance or exact engineering data.
One discreet but legible footer: AI GENERATED CONCEPT.
No copied project name, watermark, interface or page number.

DELIVERABLE
One complete full-canvas presentation board with clear hierarchy and consistent
target-building identity. No surrounding mockup frame.
```

“保持一致”是生成要求，不是已验证事实。结果检查需指出实际漂移和不合理图示。用户另有文案、真实图纸、禁止补画或双图参考要求时优先遵循。
