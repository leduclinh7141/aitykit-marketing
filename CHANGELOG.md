## [1.0.1](https://github.com/truongtv22/claudekit-engineer/compare/v1.0.0...v1.0.1) (2025-11-26)


### 🐞 Bug Fixes

* disable send release to discord ([4e42477](https://github.com/truongtv22/claudekit-engineer/commit/4e42477c8b99e4c2aecf42113162a782307c58c2))

## 1.0.0 (2025-11-26)


### 🚀 Features

* update repo ([febd801](https://github.com/truongtv22/claudekit-engineer/commit/febd801081408f5bcfa8312c9aaaca635e252085))

## [1.14.8](https://github.com/claudekit/claudekit-engineer/compare/v1.14.7...v1.14.8) (2025-11-17)


### 🐞 Bug Fixes

* modularization hook continuation ([7820f08](https://github.com/claudekit/claudekit-engineer/commit/7820f08c0351221cb9f010d1319eed4620c8b739))

## [1.14.7](https://github.com/claudekit/claudekit-engineer/compare/v1.14.6...v1.14.7) (2025-11-16)


### 🐞 Bug Fixes

* **mcp-management:** resolve subprocess hangs and signal handling ([4edb1f8](https://github.com/claudekit/claudekit-engineer/commit/4edb1f8842f41a1b3a58a2edaccc3c6752a04cec))


### 📚 Documentation

* **mcp-management:** add GEMINI.md configuration and update skill documentation ([59a1f80](https://github.com/claudekit/claudekit-engineer/commit/59a1f8071fd9bc1fbb16de9b2ea56336f721ad18))


### ♻️ Code Refactoring

* **hooks:** replace blocking prompt hook with modularization command hook ([6d6d750](https://github.com/claudekit/claudekit-engineer/commit/6d6d750512327d57da22cae82a6b4c1ea4d4a16b))

## [1.14.6](https://github.com/claudekit/claudekit-engineer/compare/v1.14.5...v1.14.6) (2025-11-16)


### 🐞 Bug Fixes

* `fast` commands should skip code reviewing ([7573bc8](https://github.com/claudekit/claudekit-engineer/commit/7573bc85806cbdba40104a49bf29e0e4822b854b))
* `planning` skills should respect `development-rules.md` ([b096874](https://github.com/claudekit/claudekit-engineer/commit/b096874fb48a853b71c8cc9d16e196d3d4b9ce53))
* hook script path resolution fails when Claude changes directories ([a6a0ecd](https://github.com/claudekit/claudekit-engineer/commit/a6a0ecd38b4bfa303aacddb7ad2602fbae6f4857))
* modular extration hook ([0293c9f](https://github.com/claudekit/claudekit-engineer/commit/0293c9f8b10e72bc5f4325f4f8312c94d85acc42))
* update development rules with name convention ([9dfcb85](https://github.com/claudekit/claudekit-engineer/commit/9dfcb85f262291471fc925c989abc4bc027895ed))


### ⚡ Performance Improvements

* `debugger` subagent should consume less tokens ([abc5635](https://github.com/claudekit/claudekit-engineer/commit/abc5635c4ef708929b5335c2a65f7be71585d0b5))

## [1.14.5](https://github.com/claudekit/claudekit-engineer/compare/v1.14.4...v1.14.5) (2025-11-16)


### 🐞 Bug Fixes

* add token count to repomix skill ([7fac84f](https://github.com/claudekit/claudekit-engineer/commit/7fac84f9d22b4acdf2b7c64268c6a00dd81ef3dc))
* get all test suite of skills passed ([6f2fe21](https://github.com/claudekit/claudekit-engineer/commit/6f2fe216df8e522a874e67394cb4e495d79fcbfc))


### ⚡ Performance Improvements

* optimize `docs-seeker` skills to be more token efficient ([840dcf3](https://github.com/claudekit/claudekit-engineer/commit/840dcf3ff1db7748d0df669ab16b2443947dd078))

## [1.14.4](https://github.com/claudekit/claudekit-engineer/compare/v1.14.3...v1.14.4) (2025-11-15)


### 🐞 Bug Fixes

* correct tools of `git-manager` agent ([5ad40eb](https://github.com/claudekit/claudekit-engineer/commit/5ad40eb8cb92563f8ea279d32e26d1fe45607059))


### ⚡ Performance Improvements

* new skills - `frontend-design` from Anthropic + animejs ([c1af484](https://github.com/claudekit/claudekit-engineer/commit/c1af484d77fc33aa7cbb13ee2c0a2077dfd13699))
* new skills - `threejs` fỏ 3D implementation ([b76ef56](https://github.com/claudekit/claudekit-engineer/commit/b76ef5674e25854b815f98c7c1f2da58c0c8e316))

## [1.14.3](https://github.com/claudekit/claudekit-engineer/compare/v1.14.2...v1.14.3) (2025-11-14)


### 🐞 Bug Fixes

* git-manager should use `main` branch instead of `master` ([b80c358](https://github.com/claudekit/claudekit-engineer/commit/b80c358e6f3232d2a97f1433493e0632e345e3b2))
* improve `/plan` output structure ([819cac2](https://github.com/claudekit/claudekit-engineer/commit/819cac240fd6dca75f85d35d4be29a16eb516687))
* unicode encoding error in gemini_batch_process.py ([14868da](https://github.com/claudekit/claudekit-engineer/commit/14868dac035e9af2520c8e9d97b92c78394f2229))


### ⚡ Performance Improvements

* `/plan` now utilize enhanced prompt ([10f6444](https://github.com/claudekit/claudekit-engineer/commit/10f6444cc5fdeee469e4d3a4aa87f125e833bd83))
* improve design commands ([7478768](https://github.com/claudekit/claudekit-engineer/commit/74787681955a4033f62d354519eb9d3f46168cc5))
* new skills - `aethetic` with design principles and templates ([7784c9f](https://github.com/claudekit/claudekit-engineer/commit/7784c9f5886bf29e37a3465993b239da5f79566c))
* new skills - `frontend-development` ([0b22630](https://github.com/claudekit/claudekit-engineer/commit/0b226305f4a588e7dde722256335b46cc501b100))
* new skills - `payment-integration` with Polar & SePay ([ca87645](https://github.com/claudekit/claudekit-engineer/commit/ca87645582a73214d8b209ea279abdd0406a2718))
* reduce token usage of `/plan:*` commands ([3cd1254](https://github.com/claudekit/claudekit-engineer/commit/3cd1254953b29d73fb14f2038eed241483097a46))
* respect core principles of claudekit ([1b33947](https://github.com/claudekit/claudekit-engineer/commit/1b3394797758c476a6368818e316fa2e77f3e707))

## [1.14.2](https://github.com/claudekit/claudekit-engineer/compare/v1.14.1...v1.14.2) (2025-11-13)


### 🐞 Bug Fixes

* correct `.mcp.json` path of `mcp-management` skills ([74035a9](https://github.com/claudekit/claudekit-engineer/commit/74035a92204be68dab58ef0bcfe58b3bc4e4d711))


### ⚡ Performance Improvements

* enhance speed of `/cook` and scouting process ([f6c02ec](https://github.com/claudekit/claudekit-engineer/commit/f6c02ecc91dba57f6792d7d6b428cc0a0886a2d1))
* new command: `/cook:fast` -> no research, only plan & code ([38cf7bf](https://github.com/claudekit/claudekit-engineer/commit/38cf7bf791344f7f1abdab14bf2089875e1c5db9))
* new command: `/plan:fast` -> no research, only scout and generate plans ([8c309b1](https://github.com/claudekit/claudekit-engineer/commit/8c309b149b5bc383f120e09c5d00b5f76b77d15d))

## [1.14.1](https://github.com/claudekit/claudekit-engineer/compare/v1.14.0...v1.14.1) (2025-11-12)


### 🐞 Bug Fixes

* `/code` should trigger subagents and update plan progress ([47861f5](https://github.com/claudekit/claudekit-engineer/commit/47861f5db7b9b415183925ae284e908ce58f7f70))
* `/fix` should enhance prompt ([26bb7ae](https://github.com/claudekit/claudekit-engineer/commit/26bb7ae5a778b88e0a55193a842634f334dd5422))
* `/fix` should enhance user prompt with more details ([551702b](https://github.com/claudekit/claudekit-engineer/commit/551702ba725543311e4e085bc5ed69916492fee2))


### 📚 Documentation

* update cli package name in readme ([d486dd8](https://github.com/claudekit/claudekit-engineer/commit/d486dd8bc887bc8d6533b110b382bc9f373f66d2))

## [1.14.0](https://github.com/claudekit/claudekit-engineer/compare/v1.13.0...v1.14.0) (2025-11-11)


### 🚀 Features

* add sequential thinking MCP server to example ([05e51fb](https://github.com/claudekit/claudekit-engineer/commit/05e51fb09a2e518a30ae68b60ebe41e723bd2bc8))


### 🐞 Bug Fixes

*  `ai-multimodal` image generation issue ([e774286](https://github.com/claudekit/claudekit-engineer/commit/e774286624c4fee10b980aead9ae6aed2835b3d9))
* `/fix` will route to `/code` when the plan exists ([b371c5b](https://github.com/claudekit/claudekit-engineer/commit/b371c5be0369512eeb7044bda8a8c12a067c8c5b))
* `project-manager` subagent should use `haiku` model for token efficiency ([4e94323](https://github.com/claudekit/claudekit-engineer/commit/4e9432300033864c0fbc62bb18092b20480a5994))
* add ⚡ to `/bootstrap:*` commands ([ead01d6](https://github.com/claudekit/claudekit-engineer/commit/ead01d60630dcfb0e0ec2c738aa242bcf46e3551))
* add ⚡ to `/fix:*` commands ([5ff1f28](https://github.com/claudekit/claudekit-engineer/commit/5ff1f28aedac6a98051bfc0acfae1091bec8be32))
* add ⚡ to commands for token consumption level ([2d8fbff](https://github.com/claudekit/claudekit-engineer/commit/2d8fbff6920609abe3b3ce4a97a82bac4b7d367f))
* add back `scout-block` hook ([255e98b](https://github.com/claudekit/claudekit-engineer/commit/255e98b3c66440d3f72ead1b25082e5149b9a1d7))
* correct ⚡ in bootstrap commands ([fa47949](https://github.com/claudekit/claudekit-engineer/commit/fa479490b313e3230cd146244cfc10bd47a8c310))
* remove deprecated Gemini 2.0 model ([00c5783](https://github.com/claudekit/claudekit-engineer/commit/00c57839f7b408a17faab696ac4756e4cf841b98))
* skill filename should be uppercase ([4984fde](https://github.com/claudekit/claudekit-engineer/commit/4984fdea80601dbb0c509a24debf29616ad2ad2b))
* support statusline on windows ([1e9351a](https://github.com/claudekit/claudekit-engineer/commit/1e9351a7e887c286b3faa074ec81df3c6345fb51))
* use haiku in mcp-manager agent for token efficiency ([40832df](https://github.com/claudekit/claudekit-engineer/commit/40832df03d3cb82268d7cef4f823b46dda90c49a))


### 📚 Documentation

* add human-mcp server in `.mcp.json.example` ([c06c3f6](https://github.com/claudekit/claudekit-engineer/commit/c06c3f6daf4b564f081ef3a8fc6302e8d3e1dcd5))
* remove outdated QA test report ([26ce054](https://github.com/claudekit/claudekit-engineer/commit/26ce05429e04db20d1adf83e25769ca4d8beb3f5))
* update readme ([0a0257f](https://github.com/claudekit/claudekit-engineer/commit/0a0257f0909437e64c354daf6dfd5e1323bd94f7))
* update readme ([bf5b685](https://github.com/claudekit/claudekit-engineer/commit/bf5b685b8b5ed4467403db149a77f0b8affd2382))
* update README ([1d34f96](https://github.com/claudekit/claudekit-engineer/commit/1d34f9676e0adc964580a2ea7b160f3709f4c475))


### ⚡ Performance Improvements

* all subagents should ensure token consumption efficiency while maintain quality ([3f0e6bd](https://github.com/claudekit/claudekit-engineer/commit/3f0e6bd5bcb0aed032159ab9791e275d8ec0beae))
* enhance `/fix:*` commands ([d9729eb](https://github.com/claudekit/claudekit-engineer/commit/d9729ebb26213325d664753136888b31675cad8c))
* enhance `debugging` skills ([8c99078](https://github.com/claudekit/claudekit-engineer/commit/8c9907839ac8bc733e07e561db36278d5397bc39))
* enhance `plan` and `scout` commands ([ccf078c](https://github.com/claudekit/claudekit-engineer/commit/ccf078c175e84c640b12e47d78f61ffa39471053))
* enhance `planner`, `researcher`, `scout` subagents ([891915f](https://github.com/claudekit/claudekit-engineer/commit/891915f56fb3e7f0088bda86b238e5462ded5b3f))
* enhance `planning` & `research` skills ([e939cc3](https://github.com/claudekit/claudekit-engineer/commit/e939cc39d268ad0a4fd85fc7d872ab1ed65e0a75))
* enhance `problem-solving` skills ([d093cc6](https://github.com/claudekit/claudekit-engineer/commit/d093cc6308f04c7e09e7954c47ce0de62510d0b6))
* enhance `sequential-thinking` skills ([ea3df40](https://github.com/claudekit/claudekit-engineer/commit/ea3df400e34116efc65d35eaf918d5da12efc70f))
* enhance `skill-creator` skills ([ce128ef](https://github.com/claudekit/claudekit-engineer/commit/ce128eff7299e4c5545ce283bd60d2ce0ef84a05))
* ensure token efficiency while maintaining high quality ([966f9ba](https://github.com/claudekit/claudekit-engineer/commit/966f9babff5c3e7e9e84a780a89e170ff14b4d9d))
* improve scout with more token efficiency ([33675dc](https://github.com/claudekit/claudekit-engineer/commit/33675dc2db676814ed60eade658850010a55b3e3))
* update scout command prefer extenal tools and fallback to explore agents ([63415be](https://github.com/claudekit/claudekit-engineer/commit/63415bed7b0078cef55717d7a71296bfdf69925b))

## [1.13.0](https://github.com/claudekit/claudekit-engineer/compare/v1.12.0...v1.13.0) (2025-11-09)


### 🚀 Features

* add `/use-mcp <to-do-something>` command ([e67a4e8](https://github.com/claudekit/claudekit-engineer/commit/e67a4e8fb39e51864e43207fb5477c2328e9a142))
* **agent:** add mcp-manager subagent ([ba40491](https://github.com/claudekit/claudekit-engineer/commit/ba404913b28b1001f3b3145b0c2fbcb1a81df04c))
* **skill:** add mcp-management skill ([8f04c03](https://github.com/claudekit/claudekit-engineer/commit/8f04c0399bcf15f67a00fc843e28abde9fb6f357))


### 🐞 Bug Fixes

* consolidate image/video processing to use ai-multimodal skill ([26bd5da](https://github.com/claudekit/claudekit-engineer/commit/26bd5da5b1e8259803cc521b2ce43539822b0441))
* issue of generate images of `ai-multimodal` skills ([c1144e9](https://github.com/claudekit/claudekit-engineer/commit/c1144e938cf59db5f912e444a2861082a80bc7bd))
* issues of markdown convert in `ai-multimodal` skills ([879561e](https://github.com/claudekit/claudekit-engineer/commit/879561e45c792e9ff27b051f25a62c98d4e36d76))
* standardize output paths of `ai-multimodal` skills ([716fd25](https://github.com/claudekit/claudekit-engineer/commit/716fd256be2541d5cea4b22965407f6892b60732))


### ⚡ Performance Improvements

* planning & research skills with token efficiency ([ed040bc](https://github.com/claudekit/claudekit-engineer/commit/ed040bc5e1160014673824171333b5e290953f1a))

## [1.12.0](https://github.com/claudekit/claudekit-engineer/compare/v1.11.0...v1.12.0) (2025-11-09)


### 🚀 Features

* new skills - `backend-development` ([0c03973](https://github.com/claudekit/claudekit-engineer/commit/0c0397364c9da6141dfc3c4300cb2617183fbc2f))
* **skill:** add mobile-development with React Native, Flutter, Swift, Kotlin ([7a73b44](https://github.com/claudekit/claudekit-engineer/commit/7a73b441aa6c4085db09db85e26c144990718709))
* **skills:** add debugging references for backend and mobile development ([970c957](https://github.com/claudekit/claudekit-engineer/commit/970c9573906217a3536620643e68f30d1595824e))


### 🐞 Bug Fixes

* add `/fix` as shorthand of `/fix:fast` ([b27f5d8](https://github.com/claudekit/claudekit-engineer/commit/b27f5d8d45c9bd1bcdc6478a648d81c6ef8309c8))


### ⚡ Performance Improvements

* add emphasis on mandatory compliance with CLAUDE.md ([fca5cb5](https://github.com/claudekit/claudekit-engineer/commit/fca5cb556124b253a1b386f60efccd93e4a71976))

## [1.11.0](https://github.com/claudekit/claudekit-engineer/compare/v1.10.6...v1.11.0) (2025-11-06)


### 🚀 Features

* **chrome-devtools:** add XPath selector support with security validation ([80ec295](https://github.com/claudekit/claudekit-engineer/commit/80ec295b4a7ea07cfa54c05bbb81bf7d52891931))
* new skills - code reviewing and problem solving ([9b7472d](https://github.com/claudekit/claudekit-engineer/commit/9b7472dcc9ce282a6285a03f653dbeb0cd14020b))
* scan and review the codebase with `/review:codebase` ([6f0e881](https://github.com/claudekit/claudekit-engineer/commit/6f0e8819f952417836887b479d5d8b658130ff3e))
* **skills:** add requirements.txt files and installation guide ([b360ec0](https://github.com/claudekit/claudekit-engineer/commit/b360ec02811a9daed849419e1917b59ce3ab6121))
* **skills:** complete Phase 4 - standalone skill refactors with progressive disclosure ([9159507](https://github.com/claudekit/claudekit-engineer/commit/91595079df71afa882928e2f8501fb5005c34c98))
* **skills:** reorganize skills with progressive disclosure (Phase 1 & 2) ([21fb8bd](https://github.com/claudekit/claudekit-engineer/commit/21fb8bd88eb2e81c165295b0785898993e361003))


### 🐞 Bug Fixes

* add rules of env var respect order in skill commands ([7e8a856](https://github.com/claudekit/claudekit-engineer/commit/7e8a8566b1cc4e73f27712c9bfc7f6cc8a3463f6))
* **ai-multimodal:** correct aspect_ratio parameter structure ([241fdfe](https://github.com/claudekit/claudekit-engineer/commit/241fdfe59053594e2cfd5eda3826d21b47a3ac8c)), closes [#27](https://github.com/claudekit/claudekit-engineer/issues/27)
* removed archived skills ([b7fae05](https://github.com/claudekit/claudekit-engineer/commit/b7fae05db93508cf748b26f21e51ac086aca9d10))
* update report location of subagents ([4175850](https://github.com/claudekit/claudekit-engineer/commit/4175850029cbdde225b124d330c81dabf3cc5eab))


### 📚 Documentation

* add pull request checklist to git manager agent ([11958c3](https://github.com/claudekit/claudekit-engineer/commit/11958c31e15cc6e0e3fc2590654fe064d61e5b5b))


### 💄 Styles

* fix typo in code review ([b0f3bf9](https://github.com/claudekit/claudekit-engineer/commit/b0f3bf9bc515fee18c6d3e8b991a268fe68b8bee))


### ♻️ Code Refactoring

* **claude-code:** optimize skill with progressive disclosure (79% reduction) ([8b51d5a](https://github.com/claudekit/claudekit-engineer/commit/8b51d5a8e47328315fd0bd0ad6e996a4d17348d6))


### ⚡ Performance Improvements

* improve /skill:create and /skill:optimize ([c6a5b32](https://github.com/claudekit/claudekit-engineer/commit/c6a5b32895e372b6119c19300534ec35f1ab5850))
* improve skills activation of subagents ([c38e0e4](https://github.com/claudekit/claudekit-engineer/commit/c38e0e4d9e6c7c95e7bfedb7b77c2acf206762af))
* improve skills commands ([da004fc](https://github.com/claudekit/claudekit-engineer/commit/da004fc567c8011d5257c87bd3c4d8cb0a8ac967))
* optimize token count in README.md ([2bd1ee2](https://github.com/claudekit/claudekit-engineer/commit/2bd1ee26b806b16d5de4558dbca7ecf6494bafce))

## [1.10.6](https://github.com/claudekit/claudekit-engineer/compare/v1.10.5...v1.10.6) (2025-11-04)


### 🐞 Bug Fixes

* /ask will respond concisely and brutal honestly ([a1b2482](https://github.com/claudekit/claudekit-engineer/commit/a1b2482c3d386a748166e92fc45efa6f6f2104cc))
* **hooks:** add cross-platform scout-block with windows support ([2c0d6de](https://github.com/claudekit/claudekit-engineer/commit/2c0d6de61f46c27c783736f0ec73b86977de9647))


### ⚡ Performance Improvements

* optimize command workflows with progressive disclosure planning ([9b76f0d](https://github.com/claudekit/claudekit-engineer/commit/9b76f0d23c4c55dbae7fe664b6c314827c58820a))

## [1.10.6](https://github.com/claudekit/claudekit-engineer/compare/v1.10.5...v1.10.6) (2025-11-04)


### 🐞 Bug Fixes

* /ask will respond concisely and brutal honestly ([a1b2482](https://github.com/claudekit/claudekit-engineer/commit/a1b2482c3d386a748166e92fc45efa6f6f2104cc))
* **hooks:** add cross-platform scout-block with windows support ([2c0d6de](https://github.com/claudekit/claudekit-engineer/commit/2c0d6de61f46c27c783736f0ec73b86977de9647))


### ⚡ Performance Improvements

* optimize command workflows with progressive disclosure planning ([9b76f0d](https://github.com/claudekit/claudekit-engineer/commit/9b76f0d23c4c55dbae7fe664b6c314827c58820a))

## [1.10.6](https://github.com/claudekit/claudekit-engineer/compare/v1.10.5...v1.10.6) (2025-11-04)


### 🐞 Bug Fixes

* /ask will respond concisely and brutal honestly ([a1b2482](https://github.com/claudekit/claudekit-engineer/commit/a1b2482c3d386a748166e92fc45efa6f6f2104cc))
* **hooks:** add cross-platform scout-block with windows support ([2c0d6de](https://github.com/claudekit/claudekit-engineer/commit/2c0d6de61f46c27c783736f0ec73b86977de9647))


### ⚡ Performance Improvements

* optimize command workflows with progressive disclosure planning ([9b76f0d](https://github.com/claudekit/claudekit-engineer/commit/9b76f0d23c4c55dbae7fe664b6c314827c58820a))

## [1.10.6](https://github.com/claudekit/claudekit-engineer/compare/v1.10.5...v1.10.6) (2025-11-04)


### 🐞 Bug Fixes

* /ask will respond concisely and brutal honestly ([a1b2482](https://github.com/claudekit/claudekit-engineer/commit/a1b2482c3d386a748166e92fc45efa6f6f2104cc))
* **hooks:** add cross-platform scout-block with windows support ([2c0d6de](https://github.com/claudekit/claudekit-engineer/commit/2c0d6de61f46c27c783736f0ec73b86977de9647))


### ⚡ Performance Improvements

* optimize command workflows with progressive disclosure planning ([9b76f0d](https://github.com/claudekit/claudekit-engineer/commit/9b76f0d23c4c55dbae7fe664b6c314827c58820a))

## [1.10.6](https://github.com/claudekit/claudekit-engineer/compare/v1.10.5...v1.10.6) (2025-11-04)


### 🐞 Bug Fixes

* /ask will respond concisely and brutal honestly ([a1b2482](https://github.com/claudekit/claudekit-engineer/commit/a1b2482c3d386a748166e92fc45efa6f6f2104cc))
* **hooks:** add cross-platform scout-block with windows support ([2c0d6de](https://github.com/claudekit/claudekit-engineer/commit/2c0d6de61f46c27c783736f0ec73b86977de9647))


### ⚡ Performance Improvements

* optimize command workflows with progressive disclosure planning ([9b76f0d](https://github.com/claudekit/claudekit-engineer/commit/9b76f0d23c4c55dbae7fe664b6c314827c58820a))

## [1.10.6](https://github.com/claudekit/claudekit-engineer/compare/v1.10.5...v1.10.6) (2025-11-04)


### 🚀 Features

* **scout-block:** add cross-platform support with Node.js dispatcher (Windows/Linux/macOS/WSL)
* **scout-block:** implement comprehensive security hardening with triple-layer validation
* **scout-block:** add PowerShell implementation for native Windows support


### 🐛 Bug Fixes

* **scout-block:** fix critical command injection vulnerability in bash implementation
* **scout-block:** add comprehensive JSON structure validation to prevent bypass attacks
* **scout-block:** improve error handling and reporting across all implementations
* **scout-block:** add empty input validation to prevent malformed request bypass


### ✅ Tests

* **scout-block:** add comprehensive test suite (11 tests: 7 functional + 4 security, 100% pass rate)
* **scout-block:** add security test coverage for input validation and error handling
* **scout-block:** add integration tests for live hook execution
* **scout-block:** validate zero regressions across all platforms


### 📚 Documentation

* **scout-block:** add cross-platform documentation with Windows support guide
* **scout-block:** update hook README with testing instructions and troubleshooting
* **scout-block:** add implementation summary with security analysis and metrics
* **scout-block:** document Node.js >=18.0.0 requirement


### ⚡ Performance Improvements

* **scout-block:** optimize with triple-layer validation architecture (defense in depth)
* **scout-block:** eliminate jq dependency using Node.js for JSON parsing
* **scout-block:** maintain minimal overhead (<50ms per invocation)


### 🔒 Security

* **scout-block:** eliminate command injection attack vector (CRITICAL)
* **scout-block:** prevent validation bypass via malformed JSON (HIGH)
* **scout-block:** add type safety enforcement across all implementations (HIGH)
* **scout-block:** implement fail-secure defaults (block on error)
* **Risk Reduction:** 95% improvement (from HIGH to LOW risk)


## [1.10.5](https://github.com/claudekit/claudekit-engineer/compare/v1.10.4...v1.10.5) (2025-11-04)


### 🐞 Bug Fixes

* remove mcp mentioning ([9e8fd79](https://github.com/claudekit/claudekit-engineer/commit/9e8fd79e0baccef62b35c39bde868736eebf83d6))
* removing .env restrictions in scout-block.sh ([9204b72](https://github.com/claudekit/claudekit-engineer/commit/9204b7275b835cc16135bc8768290ba7f3650390))
* scout-external agent use official gemini-2.5-flash ([0341b3c](https://github.com/claudekit/claudekit-engineer/commit/0341b3cd3be2bae1a4f4b0343b746c031f4bf843))


### ⚡ Performance Improvements

* add skill activation requirements to workflows ([4d805d2](https://github.com/claudekit/claudekit-engineer/commit/4d805d2517a7ba926d4b3865daad448646d010b3))
* optimize commands for token saving ([40d7c50](https://github.com/claudekit/claudekit-engineer/commit/40d7c5059772ed4fa056fe5c63e84d3f1ee24dd8))

## [1.10.4](https://github.com/claudekit/claudekit-engineer/compare/v1.10.3...v1.10.4) (2025-11-02)


### ⚡ Performance Improvements

* activate skills while planning ([254cf11](https://github.com/claudekit/claudekit-engineer/commit/254cf118b9df672c15db309241fd71dd13705d4d))

## [1.10.3](https://github.com/claudekit/claudekit-engineer/compare/v1.10.2...v1.10.3) (2025-11-02)


### ⚡ Performance Improvements

* activate skills before processing workflows ([cf4254b](https://github.com/claudekit/claudekit-engineer/commit/cf4254b75f0de365455bc73806055efbc85ee145))


### 👷 CI

* exclude docs on release ([1b2ea5b](https://github.com/claudekit/claudekit-engineer/commit/1b2ea5ba6611fe770a3d4b121a0a09c27c665594))

## [1.10.2](https://github.com/claudekit/claudekit-engineer/compare/v1.10.1...v1.10.2) (2025-11-02)


### 🐛 Bug Fixes

* block scout hook should allow .env.example files ([35ca2c3](https://github.com/claudekit/claudekit-engineer/commit/35ca2c371ddb414baebdeb87a68fa8581cba5d48))
* correct scout-block settings.json ([c345232](https://github.com/claudekit/claudekit-engineer/commit/c3452321f61f34000345ee5d99c90c5bb8ef8cc6))
* improve test workflow ([3abc48c](https://github.com/claudekit/claudekit-engineer/commit/3abc48c1a4fb055307c4b3f36f4c61287b0fd08f))
* update .env.example in skill ([a1243bc](https://github.com/claudekit/claudekit-engineer/commit/a1243bcd85edcb9428845bad2e7e0b44cebf1cf9))


### 💄 Styles

* format ([86a1bca](https://github.com/claudekit/claudekit-engineer/commit/86a1bca9e5e9edc0d1f2724b0e677205e8d65e26))


### ⚡ Performance Improvements

* gemini skill should instruct user to install `pip` if not existed ([5bd3466](https://github.com/claudekit/claudekit-engineer/commit/5bd3466d9bb04e7effb6e301604fb95ae1457376))
* improve code/cook workflow with better review ([c5ac95d](https://github.com/claudekit/claudekit-engineer/commit/c5ac95d3e99d46ce939ac733c1a481b04b01ee10))
* improve docs-seeker skill speed and accuracy ([c8054c7](https://github.com/claudekit/claudekit-engineer/commit/c8054c7f4060f581a8ae3d3d8db92ef6e897be1b))

## [1.10.1](https://github.com/claudekit/claudekit-engineer/compare/v1.10.0...v1.10.1) (2025-10-31)


### 🐛 Bug Fixes

* issue of release package ([6a13152](https://github.com/claudekit/claudekit-engineer/commit/6a131522e961acbb48e443069bfaac2a572632d1))


### 👷 CI

* fix semantic release ([2f391b7](https://github.com/claudekit/claudekit-engineer/commit/2f391b7893a3b774d5a248c774bcf915d3b9c00a))

## [1.10.0](https://github.com/claudekit/claudekit-engineer/compare/v1.9.0...v1.10.0) (2025-10-31)


### 🚀 Features

* add pre-hook to block access to sensitive directories ([7520b00](https://github.com/claudekit/claudekit-engineer/commit/7520b001fbf0fc31f70777b3761b800fa0a1c3b0))
* add scout with external agentic tools back ([22ab412](https://github.com/claudekit/claudekit-engineer/commit/22ab412b801ab15bd707c7a6a17efb49d0938c3e))


### ⚡ Performance Improvements

* fix ui uses chrome devtools ([7c52520](https://github.com/claudekit/claudekit-engineer/commit/7c5252044ef8a12e48c907c99ed371a382a914db))


### 👷 CI

* update metadata ([0d45194](https://github.com/claudekit/claudekit-engineer/commit/0d45194e1af91289c3393a4149398e09ae6f765a))

## [1.9.0](https://github.com/claudekit/claudekit-engineer/compare/v1.8.1...v1.9.0) (2025-10-30)


### 🚀 Features

* add /code command with comprehensive development workflow ([3199cb2](https://github.com/claudekit/claudekit-engineer/commit/3199cb2fdc3029c8e044a38b6da3c11224b210d5))
* add API key helper to gemini-audio skill ([57370b9](https://github.com/claudekit/claudekit-engineer/commit/57370b9692140de14906d3ea3eb2163e1c3aa853))
* add API key helper to gemini-document-processing skill ([91bd816](https://github.com/claudekit/claudekit-engineer/commit/91bd816049d44c7fe3a3a78cc7c14f6f0aa46455))
* add API key helper to gemini-image-gen skill ([b55104c](https://github.com/claudekit/claudekit-engineer/commit/b55104cd3c07918834c908559f7af3c1df3482f2))
* add API key helper to gemini-video-understanding skill ([a763e01](https://github.com/claudekit/claudekit-engineer/commit/a763e01427196387a11a5a5a55aebb8677a91b62))
* add API key helper to gemini-vision skill ([bab4bac](https://github.com/claudekit/claudekit-engineer/commit/bab4bacf3e6eea0a644cac6937a5e1225dc7b280))
* add bootstrap auto command and sequential thinking skill ([2dea7bb](https://github.com/claudekit/claudekit-engineer/commit/2dea7bb0a4b98ec5c25618453225b73bc79f42fd))
* add Chrome DevTools Protocol skill ([bae8023](https://github.com/claudekit/claudekit-engineer/commit/bae80232f8f49d7736b869a1c251c8306de7807b))
* add chrome-devtools screenshot step for wireframe generation ([a37780a](https://github.com/claudekit/claudekit-engineer/commit/a37780a2e374531abac7ea9af23c60e886a62c23))
* add Cloudflare and Google Cloud Platform skills ([dcca9d2](https://github.com/claudekit/claudekit-engineer/commit/dcca9d27002444f7c143f7ad5a157658824addd7))
* add comprehensive project documentation ([9424206](https://github.com/claudekit/claudekit-engineer/commit/94242063d84a18ecf9fb81a327ec5ee270360f9e))
* add Discord notification hook and environment templates ([fbb84cc](https://github.com/claudekit/claudekit-engineer/commit/fbb84ccd034d092ba6d3ff78b8e084c5b58bf73c))
* add Docker, MongoDB, and PostgreSQL psql skills ([606a788](https://github.com/claudekit/claudekit-engineer/commit/606a788802d65fce83af82ef23743f100030d0cd))
* add environment config examples and skills documentation ([8b05b6e](https://github.com/claudekit/claudekit-engineer/commit/8b05b6e172b97e6e5dde1118f9c6c1a1c7bbed8f))
* add fast cooking command ([6dafef1](https://github.com/claudekit/claudekit-engineer/commit/6dafef195197ae61ad2b9dcb8bb0db1d70094366))
* add Gemini Audio skill for speech generation ([95616e4](https://github.com/claudekit/claudekit-engineer/commit/95616e42c887c6842686030cecacc885f2f87025))
* add Gemini Document Processing skill ([95af4bf](https://github.com/claudekit/claudekit-engineer/commit/95af4bf4181c0b65c864c93cb86ba95af70091e4))
* add Gemini Image Generation skill ([256e9d0](https://github.com/claudekit/claudekit-engineer/commit/256e9d0af8fa2fef27434471058a2f5db58e7656))
* add Gemini Video Understanding skill ([aa82e8b](https://github.com/claudekit/claudekit-engineer/commit/aa82e8b5054329f312cab2334b8ea78e3120e529))
* add Gemini Vision skill ([8bbd682](https://github.com/claudekit/claudekit-engineer/commit/8bbd682ce40104be0d65e91a767d136159307b4c))
* add shared API key helper for Gemini skills ([8e768c7](https://github.com/claudekit/claudekit-engineer/commit/8e768c702cf8659fb19f7208b87fa0f02d77be47))
* add skill fix-logs command and enhance create command ([c77525c](https://github.com/claudekit/claudekit-engineer/commit/c77525c06376119163896c406af9c3d31ff28908))
* add Vertex AI configuration options ([bbae64f](https://github.com/claudekit/claudekit-engineer/commit/bbae64f8a59457cc549dada0e2330995e28be39e))
* **chrome-devtools:** add automatic image compression to screenshot ([661ff27](https://github.com/claudekit/claudekit-engineer/commit/661ff277aabde6cf97d0ceb6498784e2456a8036))


### 🐛 Bug Fixes

* chrome devtools - console.js timeout ([803783a](https://github.com/claudekit/claudekit-engineer/commit/803783a6157e75f70d23b7f2f82f9a38f6d77cad))
* correct agent name in CI planning command ([4d718fe](https://github.com/claudekit/claudekit-engineer/commit/4d718fe81199fba3900cfc0ac7645695615569d5))
* resolve YAML parsing errors in opencode agent descriptions ([18db16b](https://github.com/claudekit/claudekit-engineer/commit/18db16bd8bbb0f9c8a3d91289f8c13839764e63e))
* standardize GEMINI_API_KEY loading order across Gemini skills ([1b60d63](https://github.com/claudekit/claudekit-engineer/commit/1b60d639d542d017555eccb86bcd1c46148a110a))
* update .gitignore patterns for docs directories ([3a12c3e](https://github.com/claudekit/claudekit-engineer/commit/3a12c3eb66fd6235ecac47b8862864c8b0039d50))
* update git-manager agent tools configuration ([e28bfb9](https://github.com/claudekit/claudekit-engineer/commit/e28bfb9d515b5ccec9425812f3a39d9b72d131b9))


### 📚 Documentation

* add Discord and Telegram notification hook documentation ([2a26e4e](https://github.com/claudekit/claudekit-engineer/commit/2a26e4eaac34d25402135c4c65e8b69ab56bf94f))
* add documentation section to README ([08afdb2](https://github.com/claudekit/claudekit-engineer/commit/08afdb22026a9c93f0e7af52cbb75f39fc2c35db))
* add environment configuration examples ([be7eb26](https://github.com/claudekit/claudekit-engineer/commit/be7eb26ff81a87c0de700c8612f49d4818837ff2))
* generating YYMMDD dates across platforms instead of model knowledge ([fd6f9cf](https://github.com/claudekit/claudekit-engineer/commit/fd6f9cf285b45787235bffd001342c42ac0f399f))
* update project documentation for Gemini API key helpers ([557e722](https://github.com/claudekit/claudekit-engineer/commit/557e722a284356bf1676339478a82962c0d7de05))


### ♻️ Code Refactoring

* migrate from Human MCP to Gemini skills across commands and agents ([91996b2](https://github.com/claudekit/claudekit-engineer/commit/91996b288d46aa8d644dbfc2ec5a3656105f7f56))
* removed human mcp, replaced with gemini skills ([15f3074](https://github.com/claudekit/claudekit-engineer/commit/15f3074f9ac25b22dfa88a9e7a1ad4efef371f3f))
* simplify scout agent to use default Explore subagents ([62d2eda](https://github.com/claudekit/claudekit-engineer/commit/62d2eda86a791d095f2478d43426582ffc412d8e))


### ⚡ Performance Improvements

* add logo generation step to bootstrap process ([27ef839](https://github.com/claudekit/claudekit-engineer/commit/27ef839a712bb3f933dc9cb283f321534cef1994))
* enhance bootstrap command with planning phase and docs ([59b12cd](https://github.com/claudekit/claudekit-engineer/commit/59b12cdb8720da9f0f9654437d97f102bff27ab2))
* enhance common API key helper with Vertex AI support ([193270e](https://github.com/claudekit/claudekit-engineer/commit/193270ef4616961c9629b29a572b3e714f805073))
* improve Gemini vision error handling and fallback behavior ([9783f17](https://github.com/claudekit/claudekit-engineer/commit/9783f172efb6702c9dba422269a77d47fcaf67b7))
* improve URL exploration in skill creation ([715fbf9](https://github.com/claudekit/claudekit-engineer/commit/715fbf90df9338ecc6a846edd8350990db21f4a1))
* refactor docs-seeker skill with enhanced structure ([c468b66](https://github.com/claudekit/claudekit-engineer/commit/c468b66f0e0d3b13c2f7d026385f3f1d3f98c1bd))
* replace eyes analyze references ([9bf194f](https://github.com/claudekit/claudekit-engineer/commit/9bf194ffa09bf54718ecf2ecd7200888d014f21e))
* update .claude/ markdown files ([be3a1aa](https://github.com/claudekit/claudekit-engineer/commit/be3a1aaa99dad56988357e80dcb0162bc81be35a))
* update hook environment variable handling and documentation ([7634e7a](https://github.com/claudekit/claudekit-engineer/commit/7634e7a9b02ef757e9110cc3d1ff81c2b5154804))

## [1.8.1](https://github.com/claudekit/claudekit-engineer/compare/v1.8.0...v1.8.1) (2025-10-29)


### ⚡ Performance Improvements

* **skill:** optimize git-manager agent token efficiency ([e8aa189](https://github.com/claudekit/claudekit-engineer/commit/e8aa189facbd9782623d046f12eb30da953e74d3))
* **skill:** optimize git-manager agent token efficiency ([ae4ddf2](https://github.com/claudekit/claudekit-engineer/commit/ae4ddf24fc101b94b7fd0e617d8d935a8e0755a2))
* **skill:** optimize git-manager token efficiency ([5c874aa](https://github.com/claudekit/claudekit-engineer/commit/5c874aaa46efd8e5716609b747977ea81ba20000))

## [1.8.0](https://github.com/claudekit/claudekit-engineer/compare/v1.7.1...v1.8.0) (2025-10-25)


### 🚀 Features

* add ffmpeg skill documentation ([4fbed9a](https://github.com/claudekit/claudekit-engineer/commit/4fbed9a3f5e977131fcc08cd22da4fb5831a03dc))
* add shadcn-ui skill documentation ([63e6a13](https://github.com/claudekit/claudekit-engineer/commit/63e6a133a70b32ab865f6a88e9d0cccb3d3ad6b4))
* new skill - Google ADK (Python) ([6833158](https://github.com/claudekit/claudekit-engineer/commit/683315838bb6d6bbf65ad718b1b0777b2c0313fb))
* new skill - NextJS ([51f7c43](https://github.com/claudekit/claudekit-engineer/commit/51f7c4388778721ce66f6a4f795c5e60c4f98ce6))
* new skill - Remix Icon ([d762c70](https://github.com/claudekit/claudekit-engineer/commit/d762c70da86643ec70f821acf92e159985a42709))
* new skill - Shopify ([299fcb4](https://github.com/claudekit/claudekit-engineer/commit/299fcb4945efbe951f756f8168014fd2832c816f))
* new skill - Tailwind V4 ([9c911df](https://github.com/claudekit/claudekit-engineer/commit/9c911df8ea2152adfe73b4458669164f7ace72a2))
* new skill - Turborepo ([efe4224](https://github.com/claudekit/claudekit-engineer/commit/efe42245b01604a402a18c2a787233fad965f940))


### 🐛 Bug Fixes

* exclude co-author by claude and update gitignore ([511c85a](https://github.com/claudekit/claudekit-engineer/commit/511c85af4d17bd0ea4b49563b0566c144c7037d9))


### 📚 Documentation

* readme and research of shopify skill ([2cadeb8](https://github.com/claudekit/claudekit-engineer/commit/2cadeb84e07edefbd74fda52413ce0c8cd7b0cc7))


### ♻️ Code Refactoring

* replace context7 MCP tool with docs-seeker skill ([e7b13b4](https://github.com/claudekit/claudekit-engineer/commit/e7b13b42e6ef327b1bffa74be848f70e21cab30f))


### ⚡ Performance Improvements

* enhance skill creation command ([4abd785](https://github.com/claudekit/claudekit-engineer/commit/4abd7856ea35959819fbab708bb30d567b68ef6c))
* improve docs seeking skill ([2486c0a](https://github.com/claudekit/claudekit-engineer/commit/2486c0ad304a429c789b5db3f3f1376b75b81da0))

## [1.7.1](https://github.com/claudekit/claudekit-engineer/compare/v1.7.0...v1.7.1) (2025-10-24)


### 🐛 Bug Fixes

* exclude co-author by claude and update gitignore ([be0b1d9](https://github.com/claudekit/claudekit-engineer/commit/be0b1d9872b783fbb0c9a5c94c80b14def4c6920))

## [1.7.0](https://github.com/claudekit/claudekit-engineer/compare/v1.6.0...v1.7.0) (2025-10-22)


### 🚀 Features

* add claude-code skill for enhanced code assistance ([7848ae4](https://github.com/claudekit/claudekit-engineer/commit/7848ae4f491d135fd7eea7599cce26ea5692757d))
* add comprehensive repomix skill documentation ([f7c6475](https://github.com/claudekit/claudekit-engineer/commit/f7c64755f2f65676d7cf2145489214793294ea17))
* add docs-seeker skill for documentation discovery and analysis ([05cbbc8](https://github.com/claudekit/claudekit-engineer/commit/05cbbc891146cd06cba04a9cab32eade6608b0b3))


### ⚡ Performance Improvements

* enhance create skill command documentation ([559fad8](https://github.com/claudekit/claudekit-engineer/commit/559fad89fa5db855bf59ec4a04ef39f19846af2f))
* improve skill creation command with better parallel exploration guidance ([5e25fbd](https://github.com/claudekit/claudekit-engineer/commit/5e25fbdcd4776c8bcf35a0a0e3fa603ffe3d826b))

## [1.6.0](https://github.com/claudekit/claudekit-engineer/compare/v1.5.0...v1.6.0) (2025-10-21)


### 🚀 Features

* add auto command and metadata.json for project tracking ([c1bcd89](https://github.com/claudekit/claudekit-engineer/commit/c1bcd89c8b6c15ffe41b46772b5bfd6358af74d9))


### ⚡ Performance Improvements

* enhance cook command workflow and add metadata generation to release pipeline ([c4fab44](https://github.com/claudekit/claudekit-engineer/commit/c4fab44bae7b415c88ba36d15c2c3df9ad3cc288))


### 👷 CI

* setup automated release workflow with metadata generation ([413e6be](https://github.com/claudekit/claudekit-engineer/commit/413e6be4a49fd8be76c79fbfeee1e84c39dadbaf))

## [1.5.0](https://github.com/claudekit/claudekit-engineer/compare/v1.4.0...v1.5.0) (2025-10-20)


### 🚀 Features

* add debugging skill framework ([98401fe](https://github.com/claudekit/claudekit-engineer/commit/98401fe637f3b9c7b6b9c10d4a7aff4bcba672de))
* add imagemagick skill for image processing operations ([fa7b1e6](https://github.com/claudekit/claudekit-engineer/commit/fa7b1e6804f2dbf87c7efcf2f4ea63541cb1c68d))
* add new bootstrap auto command, skill create command, and better-auth skill ([10810ba](https://github.com/claudekit/claudekit-engineer/commit/10810bac6aa73b3f43789421ea7e996e1c0c2c15))
* add problem-solving skill framework ([fe63314](https://github.com/claudekit/claudekit-engineer/commit/fe63314c51f27eb164511929c66b07dbb1481271))


### ♻️ Code Refactoring

* update scout command and gitignore patterns ([d73d29b](https://github.com/claudekit/claudekit-engineer/commit/d73d29b7099364fd18c69cb2e25e20444b9ce02b))


### ⚡ Performance Improvements

* refine command descriptions and workflow processes ([3ac572d](https://github.com/claudekit/claudekit-engineer/commit/3ac572d06cf7e9776de17f3d52fe4f7bb207375e))
* update agent and command configurations ([18a211a](https://github.com/claudekit/claudekit-engineer/commit/18a211a950a77cae1a0ec114effff70bdb5ff782))
* update skill creation command and better-auth skill documentation ([4de0de1](https://github.com/claudekit/claudekit-engineer/commit/4de0de1a974a2c633f04b9445edeee43b8da7777))

## [1.4.0](https://github.com/claudekit/claudekit-engineer/compare/v1.3.1...v1.4.0) (2025-10-18)


### 🚀 Features

* add Claude skills directory with document processing and MCP tools ([563f0ce](https://github.com/claudekit/claudekit-engineer/commit/563f0ce90d37918c09039218e83ca80dd5d237ab))

## [1.3.1](https://github.com/claudekit/claudekit-engineer/compare/v1.3.0...v1.3.1) (2025-10-17)


### ⚡ Performance Improvements

* add argument-hint to command files for better CLI argument display ([d856c69](https://github.com/claudekit/claudekit-engineer/commit/d856c69beefa2a594481481947eff7683532db25))

## [1.3.0](https://github.com/claudekit/claudekit-engineer/compare/v1.2.0...v1.3.0) (2025-10-17)


### 🚀 Features

* add CRO content analysis and planning commands ([a99cbba](https://github.com/claudekit/claudekit-engineer/commit/a99cbba75fd4842e9b6e54bab11366eaa1d6f375))
* add pr command for creating pull requests ([8f9ea9c](https://github.com/claudekit/claudekit-engineer/commit/8f9ea9cdac6898cb575daf49ae57a9c0fa959650))


### ⚡ Performance Improvements

* enhance git-manager workflow process ([443740d](https://github.com/claudekit/claudekit-engineer/commit/443740db9a116035ec50cf6113a75ba060d6e4ab))
* enhance report writing guidelines in plan command ([3e8430a](https://github.com/claudekit/claudekit-engineer/commit/3e8430a06bfa0d298fb9c15e07a71a05db530c78))

## [1.2.0](https://github.com/claudekit/claudekit-engineer/compare/v1.1.2...v1.2.0) (2025-10-17)


### 🚀 Features

* add UI fix command ([356ce49](https://github.com/claudekit/claudekit-engineer/commit/356ce49294023aa19418c0cd2550156a35046093))


### 🐛 Bug Fixes

* correct typo in ClaudeKit package label ([e16955b](https://github.com/claudekit/claudekit-engineer/commit/e16955b1c088d0e6e43961ac1a953bc4631a7361))


### ⚡ Performance Improvements

* remove layout fix command ([265b9ed](https://github.com/claudekit/claudekit-engineer/commit/265b9edf28c5ec99b8f3e657ee455723b1da32d2))
* update design guideline references ([0ef871d](https://github.com/claudekit/claudekit-engineer/commit/0ef871d47fca3cf1f5e1a7b446ba9d0f3773ebe6))
* update polar and add sepay command ([16c7ee0](https://github.com/claudekit/claudekit-engineer/commit/16c7ee09d80e225200e7b907c0013e162c1aac53))

## [1.1.2](https://github.com/claudekit/claudekit-engineer/compare/v1.1.1...v1.1.2) (2025-10-17)


### 🐛 Bug Fixes

* enforce concise reporting ([775757d](https://github.com/claudekit/claudekit-engineer/commit/775757d39a263cd301c69fb58469852a2bb20a53))
* update bootstrap command guidelines ([d5eb6fb](https://github.com/claudekit/claudekit-engineer/commit/d5eb6fbd826068c2c16161eada52534af9c422e0))
* update claude guidelines (CLAUDE.md) ([1916093](https://github.com/claudekit/claudekit-engineer/commit/1916093c217b21ff03278aac52e0783e187819c7))


### 📚 Documentation

* enforce concise reporting ([8f08867](https://github.com/claudekit/claudekit-engineer/commit/8f08867f051d7f1d5c75bbdd4eec59699913e6fb))
* update claude guidelines ([252115b](https://github.com/claudekit/claudekit-engineer/commit/252115bca0b704f5c0a47e44a3e04ee541fbd382))
* update repository URLs after transfer to claudekit organization ([4cc7dba](https://github.com/claudekit/claudekit-engineer/commit/4cc7dba5fcb212a3ee36487901319fbd02f96789))

## [1.1.1](https://github.com/mrgoonie/claudekit-engineer/compare/v1.1.0...v1.1.1) (2025-10-16)


### 🐛 Bug Fixes

* improve "bootstrap" command ([3cc1be7](https://github.com/mrgoonie/claudekit-engineer/commit/3cc1be74a404f83626b7ec19f47ee54a610fbe28))


### 📚 Documentation

* add comprehensive command reference guide for ClaudeKit ([9e6b032](https://github.com/mrgoonie/claudekit-engineer/commit/9e6b0324d72a23ca4cff9acd17b7942def89c05e))
* update UI/UX designer agent tools and workflow documentation ([ccc4ebb](https://github.com/mrgoonie/claudekit-engineer/commit/ccc4ebbb51b60adb608a359e2414b336de084a78))

## [1.1.0](https://github.com/mrgoonie/claudekit-engineer/compare/v1.0.0...v1.1.0) (2025-10-09)


### 🚀 Features

* add Claude command content files ([a21de9b](https://github.com/claudekit/claudekit-engineer/commit/a21de9bf5faec2c3cf7b1d6f0775323f9eb7ea86))
* add copywriter agent and update init documentation ([8a2611a](https://github.com/claudekit/claudekit-engineer/commit/8a2611a0deee69ea7a826dc46c58cc0fadde838e))
* add journal-writer and scout agents ([2693cbc](https://github.com/claudekit/claudekit-engineer/commit/2693cbc46c9f74acf2dc28038ef19d6ddc6870e0))
* add scout command for parallel codebase search using multiple agents ([0de0e1a](https://github.com/claudekit/claudekit-engineer/commit/0de0e1a1eecbaa6fd64c88e6aa8ddca24ce3e842))

## 1.0.0 (2025-10-08)


### 🚀 Features

* add automated release system with semantic versioning ([00121c5](https://github.com/claudekit/claudekit-engineer/commit/00121c50a7bf83c3eb49aa123f6092e698c1da71))
* add Claude and OpenCode agent configurations ([5ce39d8](https://github.com/claudekit/claudekit-engineer/commit/5ce39d8de6a5768f7320021d9f9f646b67552ae6))
* add design and documentation command configurations ([060a9d1](https://github.com/claudekit/claudekit-engineer/commit/060a9d1e1e9d2bffa82481b7b214748af0a3b548))
* enhance design analysis with font prediction and positioning ([25b5a6e](https://github.com/claudekit/claudekit-engineer/commit/25b5a6e0541175bc138ddfb16d0cd805ba16ef3c))
* enhance design workflow with detailed analysis specs ([fc88236](https://github.com/claudekit/claudekit-engineer/commit/fc882360ea7852d51afe7af91055c7288b55fe1a))


### 🐛 Bug Fixes

* disable NPM publishing by default in semantic-release ([ab7775e](https://github.com/claudekit/claudekit-engineer/commit/ab7775e295f2c091974fcaae1b432686841bd4a0))
* remove npm cache dependency from GitHub Actions workflow ([26cf848](https://github.com/claudekit/claudekit-engineer/commit/26cf8488c9bb1f7b9becef233daeae1875625923))
* skip Husky commit hooks in CI environment ([b1332f5](https://github.com/claudekit/claudekit-engineer/commit/b1332f50f9d41f6bf27b9a76e35f1e0d240d64d2))
* update agent configurations and documentation ([7951821](https://github.com/claudekit/claudekit-engineer/commit/7951821e8c3a691d4a33728edf40f6964b80ff15))
* update CI and command configurations ([8569da4](https://github.com/claudekit/claudekit-engineer/commit/8569da47d52700a2812199d4a512905ec4710650))


### 📚 Documentation

* expand update command to include README and support additional requests ([c8c1677](https://github.com/claudekit/claudekit-engineer/commit/c8c1677a0cacfc668bb3ebdd7d47cea66ca1fe80))

# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

This changelog is automatically generated by [semantic-release](https://github.com/semantic-release/semantic-release) based on [Conventional Commits](https://conventionalcommits.org/).

## Types of Changes

- 🚀 **Features** - New features
- 🐛 **Bug Fixes** - Bug fixes
- 📚 **Documentation** - Documentation changes
- 💄 **Styles** - Code style changes
- ♻️ **Code Refactoring** - Code refactoring
- ⚡ **Performance Improvements** - Performance improvements
- ✅ **Tests** - Test additions/changes
- 🏗️ **Build System** - Build system changes
- 👷 **CI** - CI configuration changes

## How to Contribute

Please use [Conventional Commits](https://conventionalcommits.org/) format for your commit messages:

- `feat: add new feature` - for new features
- `fix: resolve bug in authentication` - for bug fixes
- `docs: update README with new examples` - for documentation
- `refactor: simplify user service logic` - for refactoring
- `test: add unit tests for user service` - for tests
- `ci: update GitHub Actions workflow` - for CI changes

---

*Releases and changelogs are automatically generated when changes are pushed to the main branch.*
