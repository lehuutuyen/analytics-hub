# ANALYTICS HUB — Workspace Rules

**GitHub:** https://github.com/lehuutuyen/analytics-hub

## VAI TRÒ

Trung tâm phân tích dữ liệu & chiến lược tăng trưởng. Biến data thô từ GSC, Clarity, YouTube, VidIQ thành quyết định hành động.

## NGUYÊN TẮC

1. **Data-driven only.** Mọi nhận định phải kèm số liệu cụ thể. Không suy đoán.
2. **Action-oriented.** Mỗi báo cáo phải kết thúc bằng danh sách hành động cụ thể, sắp theo ưu tiên.
3. **Honest numbers.** Báo cáo số thực, không làm đẹp. Traffic thấp thì nói thấp.
4. **Cross-channel thinking.** So sánh data từ nhiều nguồn để phát hiện patterns.

## MCP ĐƯỢC SỬ DỤNG

| MCP | Dùng cho |
|---|---|
| `google-search-console` | SEO data: keywords, clicks, impressions, ranking |
| `microsoft-clarity` | UX data: sessions, dead clicks, scroll depth, Web Vitals |
| `youtube-analytics` | Channel performance: views, watch time, engagement |
| `vidiq` | Keyword research, trending, outlier detection |
| `github` | Push reports, manage files |
| `memory` | Lưu insights xuyên phiên |
| `n8n-mcp` | Automation workflows |

## QUY ƯỚC FILE

### Weekly reports
- Tên: `YYYY-WXX-report.md` (VD: `2026-W17-report.md`)
- Chứa: Snapshot tất cả kênh, so sánh week-over-week, anomalies, action items

### Action plans
- Tên: `YYYY-MM-ten-hanh-dong.md` (VD: `2026-04-fix-title-meta.md`)
- Chứa: Vấn đề (kèm data), hành động cụ thể, deadline, metric đo kết quả

### Experiments
- Tên: `YYYY-MM-ten-thu-nghiem.md`
- Chứa: Giả thuyết, cách test, kết quả, kết luận

## WORKFLOW

```
Pull data (MCP) → Phân tích → Viết report → Push GitHub
                                    ↓
                              Action plan → Thực thi → Review kết quả
```

## INSIGHT
<!-- Agent tự ghi sau mỗi phiên -->
- 22/04/2026: Báo cáo đầu tiên (Clarity + GSC 45 ngày). Phát hiện CTR collapse là nút thắt số 1. 1,130 impressions nhưng chỉ 15 clicks.
