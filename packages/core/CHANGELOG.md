# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [0.3.0](https://github.com/binier/dgraphium/compare/@dgraphium/core@0.2.0...@dgraphium/core@0.3.0) (2020-09-26)


### Bug Fixes

* **core:** `query.project(...)` not accepting `Field` primitive ([e55cea8](https://github.com/binier/dgraphium/commit/e55cea8b46b174ead3b60aa8cb9385a04846af8c))
* **core:** `QueryBuilder.withArgs(...)` overrides `func` ([dc29d35](https://github.com/binier/dgraphium/commit/dc29d35be84916023b7aec9a1389421675b1197e))
* **core:** regression for test: "should not prefix nested `EdgeBuilder` if it has no `autoType`" ([d9a2022](https://github.com/binier/dgraphium/commit/d9a2022dfeaa413bad8d0fb9e887e0a1a87ff5ef))
* **core:** setEdges and project not returning this ([027042d](https://github.com/binier/dgraphium/commit/027042debb3b9a20bed37e9ec583caaddd991f00))
* **core:** shouldn't prefix nested elements if previous edge type is undefined ([42c12ad](https://github.com/binier/dgraphium/commit/42c12ad17ab2e5ecce5cca3f0005ea98c3d2bad4))
* **core/edge-builder:** constructor crashes if edges is undefined/null ([b818968](https://github.com/binier/dgraphium/commit/b8189689f71afeb4e378cdeb5d68366b046f0879))
* **core/edge-builder:** constructor signature - make edges optional ([c3b8d78](https://github.com/binier/dgraphium/commit/c3b8d78a93b6f8de2c027637f1e851be59201410))


### Features

* **core:** add `EdgeBuilder` merging logic ([1bf1680](https://github.com/binier/dgraphium/commit/1bf1680ac4b3883f767ed02e97b05d568bb87254))
* **core:** add a way to reference self in projection ([2e831a7](https://github.com/binier/dgraphium/commit/2e831a778b51295a71d0285471ec21a413d81fee))
* **core:** add auto type option. ([de0e0f6](https://github.com/binier/dgraphium/commit/de0e0f625c5c6b6e573b1c8ea2fee12a4ba0b46f))
* **core:** add projection merging tests ([1fa0e98](https://github.com/binier/dgraphium/commit/1fa0e985b4cad388edeeb3176786c2f5e113b798))
* **core:** allow combining already combined queries ([eb2a5a8](https://github.com/binier/dgraphium/commit/eb2a5a8eca81664d47c92fdf298471d9f6253a9a))
* **core:** allow overriding edge name with: `edge.name(...)` ([98ce338](https://github.com/binier/dgraphium/commit/98ce338761090a9688cf1c40e6f9e53ef7545b0b))
* **core:** define refs in existing query if it exists in CombinedQuery ([4611b4a](https://github.com/binier/dgraphium/commit/4611b4a63f7da8c8418f3fdb84c70d7aa9020a7b))
* **core:** imeplement edge vars ([b717d19](https://github.com/binier/dgraphium/commit/b717d193f6b36ce2892ac8aae8b06be7b7b5b219))
* **core:** implement `Field` primitive ([a87362e](https://github.com/binier/dgraphium/commit/a87362ebbe13fe702c9d2b9ecf19abd423507520))
* **core:** implement a way to extract used refs ([74a4515](https://github.com/binier/dgraphium/commit/74a4515c223011db253a732e39dbe0ced163913f))
* **core:** implement a way to reference field in query ([4a4ea08](https://github.com/binier/dgraphium/commit/4a4ea089ef7961d24f2461d00f21b727600cb90b))
* **core:** implement a way to return ref in a result as a field ([3ee0300](https://github.com/binier/dgraphium/commit/3ee0300352a000d65a7255d23795294f21f3751b))
* **core:** implement aggregations ([39b7af2](https://github.com/binier/dgraphium/commit/39b7af28ce55bf6dbbf0a0ba0cf1247564d23a26)), closes [#4](https://github.com/binier/dgraphium/issues/4)
* **core:** implement building `Query` when it contains `Ref` ([48c2a5e](https://github.com/binier/dgraphium/commit/48c2a5e49dd44072533da8f6ab368d814df7833f))
* **core:** merge projection instead of overwriting ([728f17b](https://github.com/binier/dgraphium/commit/728f17b20e97b53713dd5f88fff78b78fcb81026))
* **core/operator/uid:** accept ref ([b8e28df](https://github.com/binier/dgraphium/commit/b8e28dfa15fc9a770295648795a1ef56f3185ecf))


### BREAKING CHANGES

* **core:** `query.project(...)` will now deep merge projections by default instead of
overwriting them. to overwrite instead (previous default behavior): `query.project({}, true)`.





# [0.2.0](https://github.com/binier/dgraphium/compare/@dgraphium/core@0.1.1...@dgraphium/core@0.2.0) (2020-07-24)


### Bug Fixes

* **core:** typo. combined query missing params define line ([e3793ad](https://github.com/binier/dgraphium/commit/e3793ad674368c5aee3cb27f9849914403c0077c))


### Features

* **core:** generalize `filter` into `Directive` ([a4e506b](https://github.com/binier/dgraphium/commit/a4e506b2a64f91c267219e41e2f28ee2b7c7bbe6))
* **core:** implement [@cascade](https://github.com/cascade) directive ([9d8e71e](https://github.com/binier/dgraphium/commit/9d8e71e735faaaa25bc03fc26eacfcb970a1e739)), closes [#7](https://github.com/binier/dgraphium/issues/7)
* **core:** implement `[@ignore](https://github.com/ignore)Reflex` directive ([aa4e004](https://github.com/binier/dgraphium/commit/aa4e0042041cb9db6a7b8c6d6af7b3b4d533ebeb)), closes [#8](https://github.com/binier/dgraphium/issues/8)





## [0.1.1](https://github.com/binier/dgraphium/compare/@dgraphium/core@0.1.0...@dgraphium/core@0.1.1) (2020-07-12)

**Note:** Version bump only for package @dgraphium/core





# 0.1.0 (2020-07-10)


### Bug Fixes

* **core:** `Args.params()` crash if `func` is null ([ea0ef43](https://github.com/binier/dgraphium/commit/ea0ef43166f8a28997a501c1da3dd567d78a476e))
* **core:** `EdgeBuilder.build()` crash ([c551809](https://github.com/binier/dgraphium/commit/c551809cf1537e42c99a6551b2425715181887cc)), closes [#1](https://github.com/binier/dgraphium/issues/1)
* **core:** `Param` value type not being inferred ([1a25a80](https://github.com/binier/dgraphium/commit/1a25a80251a5b5a54ce7cc42a0cef52608e17df5))
* **core:** `ParamBuilder` accepts any value ([f02f9f1](https://github.com/binier/dgraphium/commit/f02f9f13b5f29b3389c04c16e04c4048f37fbb3a))
* **core:** `params.uid`incorrect argument type ([0c0529d](https://github.com/binier/dgraphium/commit/0c0529d251ebbbbe71bca81ff60888d05f3063cd))
* **core:** `QueryBuilder.project` not chainable ([31b953c](https://github.com/binier/dgraphium/commit/31b953ca52e66c4e87b81e1bcd06baae79fe2939))
* **core:** add missing date param function ([749a8b1](https://github.com/binier/dgraphium/commit/749a8b1f2eb3e6d3b62894e3a44e0cd3598d4148))
* **core:** Dgraph doesn't support array value param ([64e9cb9](https://github.com/binier/dgraphium/commit/64e9cb9fdcd6fc6fad85422167822a31e357c134))
* **core:** hide param define line if no params ([9c76251](https://github.com/binier/dgraphium/commit/9c76251e5708e0cfa21939ad657b6d5b3516d2fa))
* **core:** make `Operator.subject` optional ([89b46c9](https://github.com/binier/dgraphium/commit/89b46c91d5462d6e663bffa0055bf8f4e3ba0375))
* **core:** multiple string params not working ([40fbff7](https://github.com/binier/dgraphium/commit/40fbff7f35effa19607a402826d71d2d1ce7993e))
* **core:** no `paramBuilders` if opvalue is array ([9f13c06](https://github.com/binier/dgraphium/commit/9f13c06576527a2685d73a8cd4f5d04a046de499))
* **core:** param values can only be string in Dgraph ([98251ca](https://github.com/binier/dgraphium/commit/98251ca4182b728e074122f449fa1171b19eefce))
* **core:** query should display parens even if no args ([f3ae838](https://github.com/binier/dgraphium/commit/f3ae83856043faa8feab2ba4bbff2264f9fc1813))
* **core:** queryStr always should be surrounded with curly brackets ([9602eb0](https://github.com/binier/dgraphium/commit/9602eb03d942810e0d8c55ee52cb4a2a5c399d46))
* **core:** remove brackets from `uid` operator ([21c8c82](https://github.com/binier/dgraphium/commit/21c8c829a98b3392fb0150afae51ba417b4cb7dc))
* **core:** remove name parameter from param types ([69f1e6b](https://github.com/binier/dgraphium/commit/69f1e6b89cdc76615bd72edcc6a7957ce71b793d))
* **core:** typo ([d19e66d](https://github.com/binier/dgraphium/commit/d19e66d0f32611808db3d096755487b2d70cc951))
* **core:** uid param gets wrapped twice ([8f2be04](https://github.com/binier/dgraphium/commit/8f2be04ef22fb3e5e2eb79a22452b0ee32e2d669))
* make transform required for `OpBuilders` ([5f6e048](https://github.com/binier/dgraphium/commit/5f6e0488f76f54ca3b7974c7227e66b9c85e9065))
* missing import ([68ab44e](https://github.com/binier/dgraphium/commit/68ab44e09483020e1160999f02af469f42555a5b))


### Features

* **core:** `Operator` can have `Uid` value ([0027e2c](https://github.com/binier/dgraphium/commit/0027e2c7cdd8aac00735bddd8dfa345288d5f92c))
* **core:** add `Args`, contains: pagination, sorting, func ([e60bc63](https://github.com/binier/dgraphium/commit/e60bc639bb3420ea5e23ff681dd1ba08714985c7))
* **core:** add `Edge` logic ([e6caa13](https://github.com/binier/dgraphium/commit/e6caa13f428773887e174b674907fee0d9c6fad1))
* **core:** add `match` operator ([d9f3cd1](https://github.com/binier/dgraphium/commit/d9f3cd19aa2ae10e053a48eca07db4875227fe76))
* **core:** add `predUid` operator (uid_in) ([4e9e1a8](https://github.com/binier/dgraphium/commit/4e9e1a892c2d1779044659124c6fa3b17df174ff))
* **core:** add `regexp` operator ([8c04a0e](https://github.com/binier/dgraphium/commit/8c04a0ed408b8eaa5d8a0ec369b90fb66ec14cec))
* **core:** add `type` operator ([e857608](https://github.com/binier/dgraphium/commit/e85760895fb77f31f7a447b46bc2fe1443169cd6))
* **core:** add `Uid` primitive and its tests ([6865a0a](https://github.com/binier/dgraphium/commit/6865a0a617d685e6eee93b80e37ac76702458112))
* **core:** add `uids` Param type ([3605478](https://github.com/binier/dgraphium/commit/360547881f1d4b49b36e7f502392fac433ca8e2b))
* **core:** add shorter way to create edge ([287d506](https://github.com/binier/dgraphium/commit/287d50647749be152daaaac073993fadc40c75bf))
* **core:** add term operators ([0bd0b97](https://github.com/binier/dgraphium/commit/0bd0b979f4f00dcca7160a7c8b2d310ea6acbaf5))
* **core:** add text operators `[any,all]OfText` ([3c4684b](https://github.com/binier/dgraphium/commit/3c4684b68e5b970dfcfc2a1fea23322cb88aa39d))
* **core:** add ways to extract params from built objects ([e49bd13](https://github.com/binier/dgraphium/commit/e49bd1397fb32f56cb4a4d8bb3b598c58fe93122))
* **core:** combine queries ([d34a1c6](https://github.com/binier/dgraphium/commit/d34a1c6a66828c57710fe6ae53bc241c6e82390a))
* **core:** convert nested edge object to Edge ([8fa3562](https://github.com/binier/dgraphium/commit/8fa3562ad01303cc3cfa14c53f7c60870dddd2ef))
* **core:** escape operator value ([4a6e52e](https://github.com/binier/dgraphium/commit/4a6e52ef406fc46ff56c462b575bf2fb924855b0))
* **core:** export operators ([e820e99](https://github.com/binier/dgraphium/commit/e820e99998743a5702ffa92603a6904713c0a99f))
* **core:** handle `Date` type operator value ([65ba3f3](https://github.com/binier/dgraphium/commit/65ba3f359580e52d84f14ceac0ee13e475b7ed6c))
* **core:** handle `Date` type param value ([eb7d1ee](https://github.com/binier/dgraphium/commit/eb7d1eea6f4d2c1e2600b884dfa1d4fcef85200f))
* **core:** implement `eq` operator ([4f6cfef](https://github.com/binier/dgraphium/commit/4f6cfef61efc44772d81ab2804a3b3c84bdb1d45))
* **core:** implement `has` operator ([7fc2a0b](https://github.com/binier/dgraphium/commit/7fc2a0b98fe098e3dd9baa215885517cd223abe8))
* **core:** implement `uid` operator ([6262e53](https://github.com/binier/dgraphium/commit/6262e53977146707fd3d3e000b2b5b8aa1f96827))
* **core:** implement comparison operators ([f99c045](https://github.com/binier/dgraphium/commit/f99c045c46ef414626871fd9f10783422ebf731e))
* **core:** implement filtering for edge ([37101cd](https://github.com/binier/dgraphium/commit/37101cd8d015e40d2ae3f6be240a94c83ed0e057))
* **core:** implement graphql parameters ([e494e2f](https://github.com/binier/dgraphium/commit/e494e2f161827a4c72eeb414eb091e31b94369b9))
* **core:** implement operator and its builder ([83c7195](https://github.com/binier/dgraphium/commit/83c7195be6dc5b066005a377c016a65343d2358e))
* **core:** implement queries ([df101a2](https://github.com/binier/dgraphium/commit/df101a2bd705522f34a2701a8e85bdc116c1b22e))
* **core:** implement way to extract paramBuilders ([018e976](https://github.com/binier/dgraphium/commit/018e976a43808df8b339210ed06c8cfff8ada0ca))
* **core:** include `arg` param in `operator.params` ([bc00801](https://github.com/binier/dgraphium/commit/bc008018fe743fe149c918cba2510809a31b63b9))
* **core:** make edge type prefixing optional ([baa8b93](https://github.com/binier/dgraphium/commit/baa8b93ff72fcacfa223ccc219bab703e4239a97))
* **core:** operator `predUid` add support for Param uid ([bb7b029](https://github.com/binier/dgraphium/commit/bb7b029909db9f3b658e4122647f732f3c4e0ba4))
* **core:** reuse same param name if same parameter ([e63c29b](https://github.com/binier/dgraphium/commit/e63c29b528f966ca1304d8a5747f0c53a0de29bd))
* **core:** separate `uid` param type ([0400f83](https://github.com/binier/dgraphium/commit/0400f83432277ee44dfbc56015aac54a3e5705e5))
* **core:** shorter way to construct `QueryBuilder` ([e4cc7e5](https://github.com/binier/dgraphium/commit/e4cc7e500db5cb6695cfa35ae50f0d51bc385592))
* **core:** support regex param value operator ([a9564a6](https://github.com/binier/dgraphium/commit/a9564a6a1fda95bcc25300338ec0b71f3dafca15))
* create ArgsBuilder ([edfbef8](https://github.com/binier/dgraphium/commit/edfbef8cfaa0dcc09a9d9d0c95fdcb7dca0deabc))
