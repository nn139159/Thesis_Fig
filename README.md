# Thesis figures

碩士論文《LLM 驅動自駕車失效模式分類與評測基準》的圖表。
本 repo **只存放圖片**，供 HackMD 等外部文件以 raw 連結引用。
分析程式碼與資料位於另一個 private repo。

## 為什麼單獨存在

主 repo 為 private，其 `raw.githubusercontent.com` 連結帶短期 token
且會過期，不適合作為長期圖床。

## 引用方式

**請釘 commit SHA，不要用 `main`**：

```
https://raw.githubusercontent.com/<user>/<repo>/<commit-sha>/figures/<name>.png
```

論文正文的數字是凍結的。若圖片網址指向 `main`，日後任何一次重繪都會
**無聲地**改掉舊版文件裡的圖，而正文數字不會跟著變——圖與數字脫節，
且不會有任何東西報錯。

## 內容說明

全部 12 張圖均由 `make_figures.py` 以 matplotlib 依**衍生統計量**
繪製，**不含 NVIDIA PhysicalAI-AV 資料集（gated）的任何原始影像**。
產生時已自動檢查繪圖腳本不含 `imshow` / `imread`。

`manifest.json` 記錄每張圖的 SHA256 與主 repo 的來源 commit。

## 圖表清單

| 檔名 | 大小 |
|---|---|
| `fig10_turn_threshold_sensitivity.png` | 117 KB |
| `fig11_kvr_mu_sensitivity.png` | 98 KB |
| `fig12_clic_baseline_decomposition.png` | 125 KB |
| `fig1_decoupling_case_591dce37.png` | 118 KB |
| `fig2_ablation_v2.png` | 144 KB |
| `fig3_nav_counterfactual.png` | 116 KB |
| `fig4_stratified_lad.png` | 75 KB |
| `fig5_no_driving_harm.png` | 131 KB |
| `fig6_coding_sensitivity.png` | 67 KB |
| `fig7_ablation_not_specific.png` | 126 KB |
| `fig8_nav_dose_response.png` | 135 KB |
| `fig9_architecture_corrected.png` | 156 KB |
