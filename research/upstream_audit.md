# Upstream audit

        - Paper anchor: OpenCompass
        - Upstream repo: https://github.com/open-compass/opencompass
        - Local clone: /Users/Rb/Documents/LLM based projects /sources/open-compass__opencompass
        - Branch: main
        - Commit: 56ee99781397d7aabc07081a985203ad0c4ecbf7
        - File count scanned: 3355
        - Text files scanned: 3334

        ## Strengths

        - Repository has a top-level README.
- Repository exposes a dedicated docs surface.
- Repository appears to include a test surface.
- Repository has GitHub Actions or another CI entry point.

        ## Findings

        - No container packaging signal detected, which makes demos and deployment less portable.
- Mixed filename conventions detected: PascalCase, kebab-case, snake_case.
- Open maintenance markers detected: FIXME in 3 file(s), TODO in 91 file(s), XXX in 7 file(s).
- Large files that may benefit from decomposition: opencompass/datasets/IFBench/instructions.py (2272 lines), opencompass/datasets/moleculariq/moleculariq_core/solver/solver.py (1999 lines), opencompass/datasets/IFBench/instructions_util.py (1654 lines).

        ## Dominant file types

        - `.py`: 3007
- `.md`: 160
- `.txt`: 128
- `.yaml`: 17
- `.yml`: 14
- `.rst`: 6
- `<none>`: 5
- `.svg`: 4

        ## Maintenance markers

        - TODO: tools/prompt_viewer.py, examples/eval_corebench_2409_chat_objective.py, examples/eval_corebench_2409_base_objective.py, opencompass/registry.py, opencompass/tasks/llm_eval.py, opencompass/tasks/base.py, opencompass/summarizers/multi_model.py, opencompass/datasets/srbench.py
- FIXME: tools/case_analyzer.py, opencompass/utils/types.py, opencompass/models/xunfei_api.py
- XXX: examples/eval_internlm3_math500_thinking.py, examples/eval_qwen3.py, opencompass/datasets/tabmwp.py, opencompass/models/huggingface_above_v4_33.py, opencompass/openicl/icl_prompt_template.py, docs/en/notes/contribution_guide.md, docs/zh_cn/notes/contribution_guide.md
