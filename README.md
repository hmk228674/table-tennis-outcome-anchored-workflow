# 以击球结果为锚点的乒乓球多模态评估与一对一多球训练闭环

Outcome-anchored table-tennis multimodal assessment and individualized multiball planning workflow

**Public method specification · Version 0.1.0 · 2026-10-10**

作者：韩明珂（Han Mingke），华南师范大学（South China Normal University）。
[ORCID: 0009-0009-3980-662X](https://orcid.org/0009-0009-3980-662X)

## 获取本版本 / Get this version

- [Zenodo version record and archive preview](https://zenodo.org/records/23274572)
- [Version-specific DOI: 10.5281/zenodo.23274572](https://doi.org/10.5281/zenodo.23274572)
- [Frozen method bundle in this repository](table-tennis-outcome-anchored-workflow-v0.1.0.zip)
- SHA-256: `405c10baaa3c17460991ceb9ac3e1cfb8c55f913356cda48838074cbcdf8f75a`

本仓库以冻结 ZIP 保存完整的16个公开文件；Zenodo存档使用同一份 ZIP。下载并解压后阅读方法说明和运行合成测试。Zenodo页面也可浏览压缩包目录。本页是发布导航，不替代压缩包内的方法协议。

## 公开了什么

方法流程、证据与训练的关联规则、能力及解释边界、隐私与版本规范、相关工作、纯合成 JSON 示例，以及20项合成结构规则测试。

流程是：核查全部输入 → 只询问缺失信息并等待 → 逐技术、逐板复核结果 → 建立个人参照 → 证据关联结论 → 教练一对一持拍发多球计划 → 报告审核 → 复测。

**不包含真实客户的姓名、视频、身体信息、肌电或力台信号、真实逐板指标及客户报告；不包含完整商业实现。** 这不是可安装的完整分析 Skill，不是已验证的自动分析系统，也不是医学诊断工具。

## 压缩包内容

```text
table-tennis-outcome-anchored-workflow/
├── README.md, AUTHORS.md, CITATION.md, CHANGELOG.md
├── LICENSE, LICENSES/
├── RELEASE_MANIFEST.json
├── docs/
│   ├── 01_method_protocol.md
│   ├── 02_evidence_and_training_schema.md
│   ├── 03_validation_and_capability.md
│   ├── 04_disclosure_privacy_versioning.md
│   └── 05_related_work_and_candidate_contributions.md
├── examples/synthetic/example_case.json
└── tests/example_rules.py, test_example_rules.py
```

## 合成规则测试

Python 3.10及以上，无需第三方包。从解压后的目录运行：

```sh
PYTHONDONTWRITEBYTECODE=1 python3 -m unittest discover -s tests -v
```

发布前20项测试通过。它们仅检查选定的结构和边界规则，不证明实际信号处理、动作识别、训练效果、匿名性、安全性或原创性。

## 许可 / Licensing

本页和校验值说明采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)。压缩包内方法文档和合成 JSON 采用 CC BY 4.0；`tests/*.py` 采用 MIT。这是按文件适用的许可，不是对任一文件任选许可；具体范围、条款链接及通知见包内 `LICENSE` 和 `LICENSES/`。二者允许符合条款的商用和改编；客户材料、完整商业实现及外部引用作品不在授权范围内。CC BY 4.0不授予专利或商标权。

## 引用 / Citation

Han, M. (2026). *Outcome-anchored table-tennis multimodal assessment and individualized multiball planning workflow* (Version 0.1.0). Zenodo. https://doi.org/10.5281/zenodo.23274572

本版本由AI协助组织、起草和检查，署名人负责审阅与内容责任。公开记录固定的是具体版本和可验证时间，不是全球首创、可专利性、科学准确性或训练效果的认证。
