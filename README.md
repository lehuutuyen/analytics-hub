# 📊 Analytics Hub

**Trung tâm phân tích dữ liệu & chiến lược tăng trưởng** cho hệ sinh thái Lê Hữu Tuyến.

---

## Định hướng

Repo này phục vụ **1 mục đích duy nhất:** Biến dữ liệu thô thành quyết định chiến lược.

Mọi data từ website, YouTube, social — đều đổ về đây để phân tích, so sánh, và chuyển thành hành động cụ thể.

**Không lưu trữ data thô.** Data thô nằm ở nguồn gốc (GSC, Clarity, YouTube Analytics). Repo này chỉ chứa **báo cáo đã phân tích** và **kế hoạch hành động** từ data đó.

---

## Nhiệm vụ cụ thể

### 1. Thu thập & Phân tích (Weekly)
- Pull data từ các MCP → generate báo cáo tổng hợp
- So sánh week-over-week, phát hiện anomalies
- Flag vấn đề cần xử lý gấp (traffic drop, CTR collapse, broken UX)

### 2. Ra quyết định chiến lược
- Từ data → viết action plans cụ thể
- Tracking: kế hoạch → thực thi → đo kết quả
- Experiment log: test A/B, thử nghiệm title/meta, nội dung mới

### 3. Growth tracking dài hạn
- Monthly deep analysis: xu hướng tổng thể
- Quarterly strategy review: điều chỉnh hướng đi
- Milestone tracking: khi nào đạt 500/1000/5000 sessions

### 4. Knowledge Base
- Tích lũy kiến thức data analytics theo module
- Mỗi module = 1 file hoàn chỉnh (Bản chất → Lý do → Chi tiết → Áp dụng)
- Phục vụ ra quyết định nhanh, không phải tra cứu lại từ đầu

---

## Báo cáo đã có

| File | Giai đoạn | Nội dung |
|---|---|---|
| [`2026-W17-baseline-report.md`](01-weekly-reports/2026-W17-baseline-report.md) | 08/03 → 21/04/2026 (45 ngày) | Baseline report — Clarity + GSC. Phát hiện CTR collapse (1.33%), 65 dead clicks trang chủ, 16 action items |

---

## Hệ sinh thái được phân tích

| Kênh | Nguồn data | Công cụ pull |
|---|---|---|
| **Website** (lehuutuyen.com) | Google Search Console | MCP `google-search-console` |
| **Website UX** | Microsoft Clarity | MCP `microsoft-clarity` |
| **YouTube** (@lehuutuyen) | YouTube Analytics API | MCP `youtube-analytics` |
| **YouTube Research** | VidIQ | MCP `vidiq` |
| **TikTok** | (Chưa kích hoạt) | — |
| **Email** | (Chưa kích hoạt) | — |
| **Social** | (Chưa kích hoạt) | — |

---

## MCP Servers cần thiết

Để Antigravity vận hành repo này, cần các MCP sau:

| MCP Server | Vai trò | Trạng thái |
|---|---|---|
| `google-search-console` | SEO: clicks, impressions, keywords, ranking, indexing | ✅ Active |
| `microsoft-clarity` | UX: sessions, dead clicks, rage clicks, scroll depth, Web Vitals | ✅ Active |
| `youtube-analytics` | Channel: views, watch time, subscribers, engagement | ✅ Active |
| `vidiq` | Research: keyword volume, competition, trending, outliers | ✅ Active |
| `github` | Push reports, manage action plans | ✅ Active |
| `memory` | Lưu insights xuyên phiên | ✅ Active |
| `notion` | Sync action plans sang Notion (nếu cần) | ✅ Active |
| `n8n-mcp` | Automation: scheduled reports, data bridge | ✅ Active |

### MCP chưa có (Roadmap):
| MCP Server | Vai trò | Khi nào cần |
|---|---|---|
| Google Sheets MCP | Data bridge cho Looker Studio | Khi traffic > 500 sessions/tháng |
| TikTok Analytics | TikTok channel data | Khi kích hoạt TikTok |

---

## Cấu trúc thư mục

```
analytics-hub/
├── README.md                    # File này
├── AGENTS.md                    # Rules cho Antigravity
├── .agents/rules/               # Rules bổ sung
│
├── 01-weekly-reports/           # Báo cáo tuần (auto-generate)
│   └── 2026-W17-baseline-report.md  ← Baseline đầu tiên
│
├── 02-strategy/                 # Tầng chiến lược
│   ├── action-plans/            # Kế hoạch hành động từ data
│   ├── experiments/             # A/B tests, thử nghiệm
│   └── reviews/                 # Post-mortem, kết quả
│
├── 03-channel-notes/            # Ghi chú bổ sung theo kênh
│   ├── website/
│   ├── youtube/
│   └── social/
│
├── 04-automations/              # Scripts, workflow exports
│   ├── n8n-workflows/
│   └── templates/               # Template báo cáo chuẩn
│
└── 05-knowledge/                # Kiến thức data analytics
    └── INDEX.md                 # Bản đồ module + trạng thái
```

---

## Quy trình vận hành

### Weekly (mỗi thứ Hai)
```
1. Antigravity pull data từ GSC + Clarity + YouTube (qua MCP)
2. Generate weekly report → push vào 01-weekly-reports/
3. Anh Tuyến review (5-10 phút)
4. Chọn actions → ghi vào 02-strategy/action-plans/
5. Thực thi trong tuần
```

### Monthly (đầu mỗi tháng)
```
1. Tổng hợp 4 weekly reports → deep analysis
2. So sánh month-over-month
3. Cập nhật strategy nếu cần
4. Review experiment results
```

---

## Visualization Roadmap

### Giai đoạn 1 — Hiện tại (traffic < 500 sessions/tháng)
- **Công cụ:** Antigravity + MCP → Markdown reports trên GitHub
- **Lý do:** Data chưa đủ lớn cho dashboard. Tập trung fix nút thắt trước.

### Giai đoạn 2 — Khi traffic > 500 sessions/tháng
- **Công cụ:** Looker Studio (free)
- **Kết nối:** GSC + YouTube native → Looker. Clarity → Google Sheets → Looker.
- **Lý do:** Data đủ lớn, cần interactive dashboard với filter, date range, drill-down.

---

## Liên kết workspace

| Repo | Quan hệ với analytics-hub |
|---|---|
| `youtube-content` | Nhận action plans về YouTube SEO, title optimization |
| `ai-learning` | Chứa MCP config, AI tools |
| `INBOX` | Command Center, nơi khởi tạo phân tích |
| `pawvibe-research` | (Tách biệt, Pawvibe có analytics riêng nếu cần) |
