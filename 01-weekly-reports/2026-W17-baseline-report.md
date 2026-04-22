# 📊 BÁO CÁO TỔNG HỢP — lehuutuyen.com
## Microsoft Clarity + Google Search Console

- **Giai đoạn:** 08/03/2026 → 21/04/2026 (45 ngày)
- **Nguồn dữ liệu:** Microsoft Clarity (non-bot) + Google Search Console API (live data)
- **Ngày lập:** 22/04/2026

---

# PHẦN A — MICROSOFT CLARITY (Hành vi người dùng trên site)

## 1. Executive Summary

| Chỉ số | Giá trị |
|---|---|
| Tổng sessions | **71** |
| Tổng page views | **144** |
| Avg session duration | **4.75 phút** |
| Avg pages/session | **1.96 trang** |
| Bounce rate | **67.6%** |
| Single-page sessions | **48/71** (67.6%) |

**Nhận định:** Website đang ở giai đoạn **pre-launch / staging**. 71 sessions trong 45 ngày (~1.6 sessions/ngày) — traffic gần như toàn bộ từ owner. Avg session duration 4.75 phút là tín hiệu tích cực — người vào đọc khá kỹ.

---

## 2. Traffic & Acquisition

### 2.1. Nguồn traffic (theo page views)

| Nguồn | Page Views | Tỷ trọng |
|---|---|---|
| lehuutuyen.com (internal) | 67 | 46.5% |
| Direct (gõ URL / bookmark) | 56 | 38.9% |
| Google (organic search) | 12 | 8.3% |
| YouTube | 6 | 4.2% |
| eClick CRM | 2 | 1.4% |
| GitHub | 1 | 0.7% |

### 2.2. Marketing channel (theo sessions)

| Channel | Sessions | Tỷ trọng |
|---|---|---|
| Direct | 34 | 69.4% |
| Organic Search | 10 | 20.4% |
| Referral | 5 | 10.2% |
| Social / Email / Paid | 0 | 0% |

### 2.3. Landing pages → Exit pages

| Landing page | Sessions vào | Exit sessions |
|---|---|---|
| `/` (Trang chủ) | 50 (70.4%) | 45 (63.4%) |
| `/post/zmot-la-gi` | 7 | 7 |
| `/mua-tien-voi-gia-chiet-khau` | 4 | 5 |
| `/my-story` | 3 | 4 |
| `/contact` | 2 | 3 |

> [!IMPORTANT]
> Trang chủ vừa là cửa vào chính vừa là cửa thoát lớn nhất. User vào → không tìm được lý do ở lại → thoát.

---

## 3. Audience Profile

### Thiết bị & Hệ điều hành

| Thiết bị | Sessions | OS phổ biến |
|---|---|---|
| 🖥️ PC | 67 (90.5%) | Windows 41, macOS 22 |
| 📱 Mobile | 7 (9.5%) | iOS 7 |

### Vị trí địa lý (Clarity)

| Quốc gia | Sessions | Top thành phố |
|---|---|---|
| 🇻🇳 Việt Nam | 51 (71.8%) | HCM 33, Hà Nội 16 |
| 🇮🇳 Ấn Độ | 15 (21.1%) | Bengaluru 11 |
| 🇺🇸 Mỹ | 3 (4.2%) | — |
| Khác | 2 (2.8%) | Taipei, KL |

### New vs Returning

| Loại | Sessions |
|---|---|
| Returning | 42 (59.2%) |
| New | 29 (40.8%) |

---

## 4. Content Performance

| Trang | Visits | Avg Duration | Scroll Depth | Dead Clicks | Rage Clicks | Đánh giá |
|---|---|---|---|---|---|---|
| `/` (Trang chủ) | 80 | 2.46 phút | — | 65 | 0 | 🔴 |
| `/my-story` | 10 | 1.12 phút | — | 3 | 0 | 🟡 |
| `/about` | 9 | 0.88 phút | 62.3% | 2 | 0 | 🟡 |
| `/contact` | 8 | 3.08 phút | 74% | 21 | **3** | 🔴 |
| `/post/zmot-la-gi` | 7 | **4.47 phút** | — | 17 | 0 | 🟡 |
| `/mua-tien-voi-gia-chiet-khau` | 7 | **5.04 phút** | **90.1%** | 0 | 0 | 🟢 |
| `/le-huu-tuyen-la-ai` | 4 | — | **97.3%** | 2 | 0 | 🟢 |
| `/404` | 3 | — | 73.3% | 1 | 0 | 🔴 |

---

## 5. UX Health Check

| Chỉ số | Giá trị | Đánh giá |
|---|---|---|
| Tổng Dead Clicks | **118** (1.66/session) | 🔴 |
| Tổng Rage Clicks | **3** (chỉ `/contact`) | 🟡 |
| Quick-back sessions | **13/71** (18.3%) | 🟡 |
| JavaScript Errors | 0 | 🟢 |

### Broken links → 404

| Ngày | Hành trình | Nguyên nhân |
|---|---|---|
| 14/04 | `/mua-tien-voi-gia-chiet-khau` → 404 | Link nội bộ hỏng |
| 27/03 | Trang chủ → "Công Thức Copywriting" → 404 | Menu/CTA hỏng |
| 25/03 | Direct → 404 | Bookmark cũ hoặc external link |

---

## 6. Web Vitals

| Trang | LCP | CLS | FID |
|---|---|---|---|
| `/` | 1.08s 🟢 | 0.060 🟢 | 0ms 🟢 |
| `/my-story` | 1.74s 🟢 | 0.049 🟢 | 0ms 🟢 |
| `/about` | 0.40s 🟢 | 0.060 🟢 | 0ms 🟢 |
| `/mua-tien-voi-gia-chiet-khau` | 1.60s 🟢 | **0.410** 🔴 | 0ms 🟢 |
| `/post/zmot-la-gi` | 0.74s 🟢 | **0.321** 🔴 | 0ms 🟢 |

> [!WARNING]
> CLS vượt ngưỡng trên 2 trang content quan trọng nhất. Ảnh hưởng trực tiếp đến SEO ranking.

---

# PHẦN B — GOOGLE SEARCH CONSOLE (Hiệu suất trên Google)

## 7. Site Snapshot — So sánh 2 giai đoạn

| Chỉ số | 45 ngày gần nhất | 45 ngày trước đó | Thay đổi |
|---|---|---|---|
| **Clicks** | 15 | 54 | 🔴 **-72.2%** (-39) |
| **Impressions** | 1,130 | 965 | 🟢 +17.1% (+165) |
| **CTR** | 1.33% | 5.6% | 🔴 -4.27 điểm |
| **Avg Position** | 8.6 | 13.4 | 🟢 Cải thiện 4.8 bậc |

> [!CAUTION]
> **Nghịch lý nghiêm trọng:** Impressions tăng 17%, position cải thiện 4.8 bậc, nhưng clicks giảm 72%. Google hiển thị nhiều hơn, ranking tốt hơn, nhưng KHÔNG AI CLICK. Vấn đề nằm ở **title tag + meta description** — không đủ hấp dẫn để người tìm kiếm click vào.

---

## 8. Top Pages theo Google

| Trang | Clicks | Impressions | CTR | Avg Position |
|---|---|---|---|---|
| `/post/zmot-la-gi` | **10** | 237 | 4.22% | 6.4 |
| `/` (Trang chủ) | 2 | 204 | 0.98% | 6.9 |
| `/le-huu-tuyen-la-ai` | 1 | 59 | 1.69% | 5.6 |
| `/post/do-dai-bai-viet-chuan-seo` | 1 | 162 | 0.62% | 7.8 |
| `/tool/dem-ky-tu-online/` | 1 | **398** | 0.25% | 9.7 |
| `/blog` | 0 | 20 | 0% | 3.5 |
| `/contact` | 0 | 36 | 0% | 7.4 |
| `/post/dem-ky-tu-online` | 0 | 30 | 0% | 7.5 |
| `/post/dem-ky-tu-online-google-dich` | 0 | 27 | 0% | 8.3 |
| `tools.lehuutuyen.com/` | 0 | 24 | 0% | 12.2 |

> [!IMPORTANT]
> **`/tool/dem-ky-tu-online/` có 398 impressions nhưng chỉ 1 click (CTR 0.25%).** Đây là trang được Google hiển thị NHIỀU NHẤT nhưng gần như không ai click. Title/meta cần viết lại gấp.

---

## 9. Top Search Queries — Keyword clusters

### Cluster 1: "Đếm ký tự online" (chiếm 38% tổng impressions)

| Query | Clicks | Impressions | Position |
|---|---|---|---|
| đếm ký tự online | 0 | 278 | 9.6 |
| demkytu | 0 | 39 | 8.2 |
| bộ đếm ký tự online | 0 | 30 | 9.7 |
| đếm số ký tự online | 0 | 15 | 10.2 |
| dđếm ký tự online | 0 | 13 | 9.5 |
| dem ky tu online | 0 | 12 | 11.6 |
| đếm kí tự online | 0 | 10 | 9.9 |
| **Tổng cluster** | **0** | **397** | **~9.7** |

**Nhận định:** 397 impressions, **0 clicks**. Ranking trang 1 (pos ~9.7) nhưng title/meta không thu hút. Đây là cơ hội lớn nhất — chỉ cần tối ưu title là có traffic ngay.

### Cluster 2: "ZMOT" (chủ đề chuyên môn)

| Query | Clicks | Impressions | Position |
|---|---|---|---|
| zmot | 4 | 55 | 12.1 |
| zmot là gì | 1 | 53 | 3.5 |
| zmot in marketing | 0 | 3 | 8.3 |
| zmot marketing | 0 | 3 | 6 |
| **Tổng cluster** | **5** | **114** | — |

**Nhận định:** Cluster hiệu quả nhất — CTR ~4.4%. "zmot là gì" rank 3.5 (gần top 3). Đẩy lên top 1-3 sẽ tăng clicks đáng kể.

### Cluster 3: Brand name

| Query | Clicks | Impressions | Position |
|---|---|---|---|
| lê hữu tuyến | 2 | 27 | 5.6 |
| hữu tuyến | 0 | 9 | 8.6 |
| lê hữu | 0 | 5 | 3.8 |

### Cluster 4: Khác

| Query | Clicks | Impressions | Position |
|---|---|---|---|
| eclick | 0 | 55 | 9.7 |
| crm | 0 | 15 | 12.9 |
| bài viết chuẩn seo bao nhiêu từ | 0 | 12 | 13.3 |

---

## 10. Traffic Drops — Chẩn đoán nguyên nhân

| Trang | Clicks hiện tại | Clicks trước | Thay đổi | Chẩn đoán |
|---|---|---|---|---|
| `/` (Trang chủ) | 2 | 19 | **-17** | 🔴 Ranking loss (pos 4.6 → 6.9) |
| `/tool/dem-ky-tu-online/` | 1 | 12 | **-11** | 🟡 CTR collapse |
| `/le-huu-tuyen-la-ai` | 1 | 9 | **-8** | 🟡 CTR collapse |
| `/post/web-dem-ky-tu` | 0 | 5 | -5 | 🟡 CTR collapse |
| `/contact` | 0 | 4 | -4 | 🟡 CTR collapse |
| `tools.lehuutuyen.com/` | 0 | 4 | -4 | 🔴 Ranking loss (pos 9.8 → 12.2) |
| `/tuyen-ngon-kinh-doanh` | 0 | 3 | -3 | 🟡 CTR collapse |
| `/ban-su-chuyen-doi` | 0 | 1 | -1 | 🟡 CTR collapse |

> [!WARNING]
> **7/9 trang mất traffic do CTR collapse** — không phải vì mất ranking. Google vẫn hiển thị nhưng title/meta không đủ hấp dẫn so với đối thủ.

---

## 11. Quick Wins — 12 keyword cơ hội

Keyword đang ranking pos 4-15, có impressions cao, chỉ cần tối ưu nhẹ là lên top:

| Keyword | Impressions | Position | Opportunity Score |
|---|---|---|---|
| đếm ký tự online | 278 | 9.6 | ⭐ 31 |
| eclick | 55 | 9.7 | ⭐ 6 |
| demkytu | 39 | 8.2 | ⭐ 4 |
| bộ đếm ký tự online | 30 | 9.7 | ⭐ 3 |
| zmot | 55 | 12.1 | ⭐ 2 |
| crm | 15 | 12.9 | ⭐ 2 |
| đếm số ký tự online | 15 | 10.2 | ⭐ 2 |
| lê hữu tuyến | 27 | 5.6 | ⭐ 1 |
| bài viết chuẩn seo bao nhiêu từ | 12 | 13.3 | ⭐ 1 |
| dem ky tu online | 12 | 11.6 | ⭐ 1 |
| dđếm ký tự online | 13 | 9.5 | ⭐ 1 |
| đếm kí tự online | 10 | 9.9 | ⭐ 1 |

---

## 12. Quốc gia — GSC vs Clarity

| Quốc gia | GSC Impressions | GSC Clicks | Clarity Sessions |
|---|---|---|---|
| 🇻🇳 Việt Nam | 1,004 (88.8%) | 14 | 51 (71.8%) |
| 🇺🇸 Mỹ | 68 (6%) | 0 | 3 (4.2%) |
| 🇮🇳 Ấn Độ | 1 | 0 | 15 (21.1%) |
| 🇹🇼 Đài Loan | 5 | 1 | 1 |
| Khác | 52 | 0 | 1 |

> [!NOTE]
> **Ấn Độ: 15 sessions trên Clarity nhưng chỉ 1 impression trên GSC.** Xác nhận traffic từ Ấn Độ KHÔNG đến từ Google Search — có thể là bot, direct access, hoặc referral. Loại khỏi phân tích traffic thực.

---

# PHẦN C — TỔNG HỢP CHIẾN LƯỢC

## 🔴 Làm ngay (1-2 ngày tới)

| # | Action | Data từ | Impact dự kiến |
|---|---|---|---|
| 1 | **Viết lại title + meta cho `/tool/dem-ky-tu-online/`** | GSC: 398 imp, CTR 0.25% | Tăng CTR lên 5% = ~20 clicks/45 ngày |
| 2 | **Viết lại title + meta cho trang chủ** | GSC: 204 imp, CTR 0.98% | Tăng brand click, giảm bounce |
| 3 | **Fix link "Công Thức Copywriting" trên trang chủ** | Clarity: dẫn đến 404 | Giữ user không rơi vào deadend |
| 4 | **Fix link nội bộ hỏng trên `/mua-tien-voi-gia-chiet-khau`** | Clarity: session 14/04 | Bảo vệ trang engagement tốt nhất |
| 5 | **Fix nút "Nhận Quà Tặng" trên trang 404** | Clarity: dead click | Tận dụng user đã lỡ rơi vào 404 |

## 🟡 Tuần này

| # | Action | Data từ | Impact dự kiến |
|---|---|---|---|
| 6 | **Tối ưu title + meta cho `/post/do-dai-bai-viet-chuan-seo`** | GSC: 162 imp, CTR 0.62% | Potential +8 clicks |
| 7 | **Fix CLS trên `/mua-tien-voi-gia-chiet-khau` (0.410)** | Clarity Web Vitals | Cải thiện SEO ranking |
| 8 | **Fix CLS trên `/post/zmot-la-gi` (0.321)** | Clarity Web Vitals | Bảo vệ trang SEO số 1 |
| 9 | **Audit 65 dead clicks trên trang chủ** | Clarity UX | Giảm frustration, tăng navigation |
| 10 | **Kiểm tra form `/contact`** | Clarity: 3 rage clicks | Đảm bảo form submit hoạt động |
| 11 | **Đẩy "zmot là gì" từ pos 3.5 lên top 1-3** | GSC Quick Wins | Keyword CTR cao nhất (7.27%) |

## 🟢 Tháng này (Growth phase prep)

| # | Action | Data từ | Impact dự kiến |
|---|---|---|---|
| 12 | **Tạo content mới cho "công cụ hỗ trợ viết bài chuẩn seo"** | GSC Content Gaps: pos 41.4 | Mở rộng topic cluster SEO tools |
| 13 | **Kích hoạt Social channel** (YouTube → site link) | Clarity: Social = 0 | Kênh traffic chủ động |
| 14 | **Thiết lập Email funnel** | Clarity: Email = 0 | Lead capture cho returning visits |
| 15 | **Gộp 3 trang đếm ký tự thành 1 trang mạnh** | GSC: 3 URLs cùng topic, dilute authority | Tập trung 455 impressions vào 1 URL |
| 16 | **Loại traffic India khỏi Clarity** | Cross-ref GSC vs Clarity | Làm sạch data phân tích |

---

> **Kết luận chiến lược từ 2 nguồn data:**
>
> **Google đang cho anh cơ hội** — 1,130 impressions, position trung bình 8.6 (trang 1). Nhưng anh đang **lãng phí 97% cơ hội** vì CTR chỉ 1.33%.
>
> **Nút thắt cổ chai số 1:** Title tag + Meta description. Không phải nội dung. Không phải kỹ thuật. Người ta thấy site trên Google nhưng không thèm click.
>
> **Nút thắt cổ chai số 2:** Trang chủ không giữ chân được ai. 65 dead clicks + bounce rate 67.6% + trang exit lớn nhất.
>
> **Chiến thuật tối ưu:** Fix title/meta cho top 3 trang có impressions cao nhất → tăng clicks gấp 3-5x mà không cần tạo thêm content mới.
