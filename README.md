    # 雾凇拼音 (个人定制版)

    本项目是基于优秀的开源拼音输入法配置 **[雾凇拼音 (rime-ice)](https://github.com/iDvel/rime-ice)** 的个人深度定制版。

    ## 🌟 关于本项目                                                                                                                                                                      

    得益于 Rime 强大的 `custom.yaml` 补丁机制，本项目在**完全保留官方核心文件**且能够**随时无缝同步上游更新**的基础上，沉淀了我个人的专属配置，主要包括：

    - 精简并专属保留的输入方案（全拼、小鹤双拼、拼音加加）
    - 自定义的候选词数量调整（8个）
    - 个性化的鼠须管（Squirrel / 雾凇拼音 Mac 端）输入法皮肤定制
    - 自定义的扩展词库与个人输入习惯调优

    ## 📦 核心源码与感谢                                                                                                                                                                  

    本项目的所有核心词库、复杂的 Lua 扩展脚本及底层拼写逻辑，均来自原作者的无私开源。强烈建议大家去原项目了解详情并点个 Star 支持作者！

    - **官方上游仓库**: [iDvel / rime-ice](https://github.com/iDvel/rime-ice)
    - **官方使用文档**: [雾凇拼音官方指南](https://dvel.me/posts/rime-ice/)

    ## 🔄 同步与更新机制                                                                                                                                                                  

    本项目配置了专属的 Git `upstream` 与特殊的合并策略。
    当需要同步官方最新的词库和核心逻辑时，执行以下操作（注：本 `README.md` 及所有的 `*.custom.yaml` 已被配置为永远保留本地版本，不用担心被官方覆盖）：

    ```bash
    git fetch upstream
    git merge upstream/main --no-edit
    git push origin main

  (或者使用配套的 Raycast 脚本一键完成同步与备份)
    ---
