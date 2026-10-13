This version contains the following changes:

- Edge Read Aloud online voices now use the new endpoint `api.msedgeservices.com` with the `Ocp-Apim-Subscription-Key` query parameter, as a workaround for the legacy `speech.platform.bing.com` endpoint returning HTTP 403. The existing `Sec-MS-GEC` token generation is unchanged.
- CI runners are pinned to `windows-2022`, because `windows-latest` now resolves to a VS2026 image that provides neither the v143 toolset nor ATL.

---

此版本包含以下改动：

- Edge 朗读在线语音改用新端点 `api.msedgeservices.com` 及查询参数 `Ocp-Apim-Subscription-Key`，作为旧端点 `speech.platform.bing.com` 返回 HTTP 403 的应急处理。原有的 `Sec-MS-GEC` 令牌生成算法保持不变。
- CI 运行器固定为 `windows-2022`，因为 `windows-latest` 现在指向 VS2026 镜像，既不提供 v143 工具集也没有 ATL。
