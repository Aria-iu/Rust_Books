# Rust 书籍索引与学习路线

按 **2026 → 2025 → 官方学习资料 → 仓库已有书籍** 整理 Rust 资源。每项包含学习方向、内容概要和访问位置；仓库已有的全部 17 份书籍均可在下表点击文件名打开。出版社条目提供购买或阅读入口，官方资料提供在线版或源码下载。

## 2026：新版与近期出版物

| 年份/状态 | 书籍或资源 | 方向 | 概要 | 访问 |
| --- | --- | --- | --- | --- |
| 2026-05（MEAP；约 70% 完成，预计 2027 年初出版） | *Embedded Software with Rust* — David Cabanis | 嵌入式 / 固件 / `no_std` | 以固件实践讲解裸机 Rust、外设访问、内存映射 I/O、定时/中断与 C 互操作，补足嵌入式学习路径。 | [Manning 官方付费购买 / 订阅后在线阅读（MEAP）](https://www.manning.com/books/embedded-software-with-rust) |
| 2026-04 | *Rust: The Practical Guide* — Nouman Azam | 入门到进阶 | 从安装、语法与所有权起步，逐步进入泛型、智能指针、并发、宏和 Web 编程，并配有练习。 | [Packt 官方付费购买（购买后可按授权下载电子书）](https://www.packtpub.com/en-us/product/rust-9781807785109) |
| 2026-03 | *The Rust Programming Language*, 3rd Edition — Steve Klabnik、Carol Nichols、Chris Krycho | 语言基础 / 工程实践 | 基于 Rust 2024 Edition，新增完整 async 章节与 Miri，结合 CLI 和多线程服务器项目解释所有权、类型、错误处理与 Cargo。 | [No Starch 官方付费购买 / 购买后阅读](https://nostarch.com/rust-programming-language-3e) |
| 2026-01 | *Rust Web Programming*, 3rd Edition — Maxwell Flitton | Web / 微服务 | 从 Rust 基础衔接服务端 Web 开发，涵盖 Axum、WebAssembly、TLS 及微服务与 nanoservice 的设计实践。 | [Packt 官方付费购买 / 购买后在线阅读](https://www.packtpub.com/en-us/product/rust-web-programming-9781835887776) |

## 2025：仍具参考价值的近作

| 年份/状态 | 书籍或资源 | 方向 | 概要 | 访问 |
| --- | --- | --- | --- | --- |
| 2025-12 | *The Rust Programming Handbook* — Francesco Ciulla | 入门 / 工程实践 | 从开发环境、核心语法和 CLI 项目入门，再延伸到所有权、并发与构建实际应用所需的 Rust 基础。 | [Packt 官方付费购买 / 购买后在线阅读](https://www.packtpub.com/en-us/product/the-rust-programming-handbook-9781836208877) |
| 2025-06 | *Refactoring to Rust* — Lily Mara、Joel Holmes | 迁移 / FFI | 面向既有代码库的渐进式迁移：以 Rust 库接入其他语言，处理安全边界、并发、HTTP 服务与 WebAssembly。 | [Manning 官方付费购买 / 订阅后在线阅读](https://www.manning.com/books/refactoring-to-rust) |
| 2025（作者页面标注 ©2025；更新状态未核实） | *Rust for C Programmers* — S. Salewski | C/C++ 转 Rust | 为熟悉 C 的系统开发者对照讲解所有权、借用、类型系统、`unsafe` 与 FFI，建立不同于手工内存管理的思维方式。 | [作者免费在线阅读](https://rust-for-c-programmers.com/) |

## 长期可用的官方 / 维护者免费资料

| 年份/状态 | 书籍或资源 | 方向 | 概要 | 访问 |
| --- | --- | --- | --- | --- |
| 持续更新（官方；Rust 2024 Edition） | *The Rust Programming Language*（官方在线版） | 入门 / 语言基础 | Rust 项目维护的入门主线，覆盖安装、所有权、trait、测试、并发与常用工程流程；适合作为第一本免费教材。 | [在线阅读](https://doc.rust-lang.org/book/) · [源码 ZIP 下载](https://github.com/rust-lang/book/archive/refs/heads/main.zip) |
| 重写中（内容可能缺失或粗糙） | *Asynchronous Programming in Rust* | async / 并发 | 以 Future、async/await 与运行时模型建立异步心智模型；官方说明正在重写，部分内容可能缺失或较粗糙，适合补充概念，实践时应结合现行运行时文档。 | [在线阅读](https://rust-lang.github.io/async-book/) · [源码 ZIP 下载](https://github.com/rust-lang/async-book/archive/refs/heads/master.zip) |
| 开源项目资料（可在线使用） | *Command Line Applications in Rust* | CLI 工具 | 以一个可工作的 CLI 为起点，讲参数、错误、测试、配置、信号、文档与发布，适合用项目巩固 Cargo。 | [在线阅读](https://rust-cli.github.io/book/) · [源码 ZIP 下载](https://github.com/rust-cli/book/archive/refs/heads/master.zip) |
| 官方工作组资料（Rust 2018 示例） | *The Embedded Rust Book* | 嵌入式 / `no_std` | 聚焦裸机与资源受限环境，涉及交叉编译、内存映射外设、中断、并发和硬件抽象；示例以 ARM Cortex-M 为主。 | [在线阅读](https://docs.rust-embedded.org/book/) · [源码 ZIP 下载](https://github.com/rust-embedded/book/archive/refs/heads/master.zip) |
| 持续更新（官方） | *The Cargo Book* | 构建 / 包管理 | 系统说明 package、依赖、workspace、profile、发布与命令行工作流，是所有 Rust 工程的常用参考。 | [在线阅读](https://doc.rust-lang.org/cargo/) |
| 持续更新（官方） | *The rustc book* | 编译器 / 工具链 | 介绍 `rustc` 的命令行选项、代码生成、lint、链接与调试相关能力，适合排查构建与编译问题。 | [在线阅读](https://doc.rust-lang.org/rustc/) |

## 仓库已有书籍索引（17 份）

以下覆盖仓库根目录中的全部 17 份书籍。点击「仓库位置」中的文件名即可打开对应 PDF。书名按现有文件名整理，具体作者、版次以文件扉页为准；MEAP 表示预览稿。

| 书籍或资料 | 方向 | 概要 | 仓库位置 |
| --- | --- | --- | --- |
| *Command-Line Rust* | CLI / 项目实战 | 通过多个命令行项目训练参数解析、错误处理、文件处理、测试与发布流程。 | [Command-Line Rust A Project-Based Primer for Writing Rust CLIs_9781098109431.pdf](./Command-Line%20Rust%20A%20Project-Based%20Primer%20for%20Writing%20Rust%20CLIs_9781098109431.pdf) |
| *Data Analysis with Rust Notebooks* | 数据分析 / Notebook | 将 Rust 用于可复现实验、数据处理和交互式 notebook 工作流。 | [Data Analysis with Rust Notebooks (Dr. Shahin Rostami) (Z-Library).pdf](./Data%20Analysis%20with%20Rust%20Notebooks%20%28Dr.%20Shahin%20Rostami%29%20%28Z-Library%29.pdf) |
| *GUI Development with Rust and GTK 4* | 桌面 GUI | 使用 GTK 4 构建 Rust 图形界面，覆盖控件、事件、状态与桌面应用组织。 | [GUI development with Rust and GTK 4.pdf](./GUI%20development%20with%20Rust%20and%20GTK%204.pdf) |
| *Hands-On Concurrency with Rust* | 并发 / 性能 | 围绕线程、消息传递、共享状态与并行算法构建内存安全的高效并发程序。 | [Hands-On Concurrency with Rust Confidently build memory-safe, parallel, and efficient software in Rust (Brian L. Troutwine) (Z-Library).pdf](./Hands-On%20Concurrency%20with%20Rust%20Confidently%20build%20memory-safe%2C%20parallel%2C%20and%20efficient%20software%20in%20Rust%20%28Brian%20L.%20Troutwine%29%20%28Z-Library%29.pdf) |
| *RISC-V Reader*（中文版） | 计算机体系结构 | RISC-V 指令集与软硬件接口参考，可辅助理解 Rust 嵌入式与底层开发环境。 | [RISC-V-Reader-Chinese-v2p12017.pdf](./RISC-V-Reader-Chinese-v2p12017.pdf) |
| *Refactoring to Rust*（MEAP） | 迁移 / FFI | 面向遗留系统的渐进式 Rust 改造，重点是边界设计、互操作和安全替换。 | [Refactoring to Rust MEAP V05 (Lily Mara) (Z-Library).pdf](./Refactoring%20to%20Rust%20MEAP%20V05%20%28Lily%20Mara%29%20%28Z-Library%29.pdf) |
| *Rust Design Patterns*（MEAP） | 设计模式 / 架构 | 汇集 Rust 惯用模式与可复用设计方案，适合在掌握基础后提升工程组织能力。 | [Rust Design Patterns (MEAP V02) (Brenden Matthews) (Z-Library).pdf](./Rust%20Design%20Patterns%20%28MEAP%20V02%29%20%28Brenden%20Matthews%29%20%28Z-Library%29.pdf) |
| *Rust in Practice*, 2nd Edition | 工程实战 / 系统编程 | 通过真实工程主题练习网络、系统接口、可靠性与生产级 Rust 开发。 | [Rust In Practice, Second Edition (Rick Tim).pdf](./Rust%20In%20Practice%2C%20Second%20Edition%20%28Rick%20Tim%29.pdf) |
| *Rust Web Development* | Web 后端 | 介绍以 Rust 构建 Web 服务的路由、请求处理、数据层与部署基础。 | [Rust Web Development_9781617299001.pdf](./Rust%20Web%20Development_9781617299001.pdf) |
| *Rust 参考手册*（中文版） | 语言参考 | 面向查阅的语言规范类资料，适合确认语法、类型、表达式和语义细节。 | [Rust 参考手册 中文版.pdf](./Rust%20%E5%8F%82%E8%80%83%E6%89%8B%E5%86%8C%20%E4%B8%AD%E6%96%87%E7%89%88.pdf) |
| *Rust 权威指南* | 入门 / 语言基础 | 以所有权、借用、类型系统、错误处理和并发为主线的系统入门材料。 | [Rust权威指南.pdf](./Rust%E6%9D%83%E5%A8%81%E6%8C%87%E5%8D%97.pdf) |
| *Rust 程序设计* | 入门 / 编程基础 | 从基本语法、控制流和数据结构进入 Rust 编程，适合补齐语言起步知识。 | [Rust程序设计.pdf](./Rust%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1.pdf) |
| *The Embedded Rust Book* | 嵌入式 / `no_std` | 裸机 Rust、交叉编译、外设访问、中断与硬件抽象的入门资料。 | [The Embedded Rust Book.pdf](./The%20Embedded%20Rust%20Book.pdf) |
| *The Embedded Rust Book*（中文版） | 嵌入式 / `no_std` | 上述嵌入式资料的中文版本，便于快速理解 Cortex-M 与裸机开发概念。 | [The Embedded Rust Book＿Ｃｈｉｎｅｓｅ.pdf](./The%20Embedded%20Rust%20Book%EF%BC%BF%EF%BC%A3%EF%BD%88%EF%BD%89%EF%BD%8E%EF%BD%85%EF%BD%93%EF%BD%85.pdf) |
| *The rustc book* | 编译器 / 工具链 | `rustc` 选项、代码生成与编译诊断的参考资料。 | [The rustc book.pdf](./The%20rustc%20book.pdf) |
| *精通 Rust（第 2 版）* | 进阶 / 工程实践 | 面向已有基础的进阶主题，适合深化类型、抽象、并发与工程化能力。 | [精通Rust（第2版）.pdf](./%E7%B2%BE%E9%80%9ARust%EF%BC%88%E7%AC%AC2%E7%89%88%EF%BC%89.pdf) |
| *通过例子学 Rust*（中文版） | 示例驱动入门 | 用可运行的小例子讲解语言特性，适合配合主线教材快速练习。 | [通过例子学 Rust 中文版.pdf](./%E9%80%9A%E8%BF%87%E4%BE%8B%E5%AD%90%E5%AD%A6%20Rust%20%E4%B8%AD%E6%96%87%E7%89%88.pdf) |

## 按目标选择阅读路径

- **第一次学习 Rust：** 先读官方在线版 *The Rust Programming Language*；希望用最新付费实体/电子版系统学习，可选其 2026 第 3 版。
- **已有 C/C++ 背景：** 用 *Rust for C Programmers* 建立所有权与借用的对照思维，再读 *Refactoring to Rust* 学习渐进迁移和 FFI。
- **异步或高并发服务：** 在掌握官方主线后，可用重写中的 *Asynchronous Programming in Rust* 补齐概念；实战时再对照所选运行时（如 Tokio）的现行官方文档。
- **命令行工具：** 以 *Command Line Applications in Rust* 或仓库中的 *Command-Line Rust* 实作一个可发布 CLI，并随时查阅 *The Cargo Book*。
- **Web、API 与微服务：** 选择 2026 年的 *Rust Web Programming*, 3rd Edition，并可参考仓库中的 *Rust Web Development*。
- **嵌入式、`no_std` 或构建工具链：** 硬件开发先读 *The Embedded Rust Book*，再按需选 *Embedded Software with Rust*（MEAP，未完稿）；工程配置与编译诊断结合 *The Cargo Book* 和 *The rustc book*。

## 使用说明

- 书籍的出版时间和电子版可用性以其出版方页面为准；MEAP 条目明确标注未完稿和预计出版时间，避免将预发行误认为正式发售。
- 商业书籍仅可在出版方完成付费购买或订阅后，按其授权阅读或下载；源码 ZIP 链接只用于开源资料源码。请遵守对应购买条款与许可证。
- 如发现链接失效、出版信息更新，欢迎提交 issue 或 PR，并优先提供作者、出版社或 Rust 项目的原始链接。
