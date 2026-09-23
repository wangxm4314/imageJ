# imageJ — Fiji/ImageJ 荧光定位分析工作区

使用 Fiji/ImageJ 对结核分枝杆菌 novel ORF 目的蛋白的 **mScarlet3 荧光标记图像**进行亚细胞定位分析。

## 目录结构

| 路径 | 说明 |
| --- | --- |
| `raw_image/` | 仪器导出的原始显微图像（OME-TIFF），按课题/批次命名子目录 |
| `raw_image/wxm_novel_orf/` | wxm_novel_orf 课题的原始图像与分析任务说明（`cue_word.md`） |
| `scripts/` | Fiji/ImageJ 宏（`.ijm`）与 Python 分析脚本 |
| `results/` | 分析输出（分割、定位结果、图表等），目录保留、内容不入库 |

## 数据

- 原始图像位于 `raw_image/wxm_novel_orf/`：
  - `2026-06-23_Batch01__B02_r1-c0_20260623_191859.ome.tif`
  - `2026-06-23_Batch01__B05_r0-c2_20260623_191652.ome.tif`
- 荧光通道：mScarlet3（红光）；分析目标：观察目的蛋白在菌体内的定位。

## 分析任务

见 [`raw_image/wxm_novel_orf/cue_word.md`](raw_image/wxm_novel_orf/cue_word.md)。

## 备注

- Fiji 临时文件、系统文件以及 `results/` 下的输出已通过 `.gitignore` 忽略。
- 现有原始图像（约 32 MB）直接保留在仓库中；后续更大规模的数据建议使用 Git LFS 或外部存储管理。
