---
type: tool
tags: [ads, utm, tracking, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14a - ADS Facebook]]", "[[Khối 14b - ADS Google]]", "[[Khối 14c - ADS TikTok]]", "[[Khối 14d - ADS YouTube]]"]
---

# UTM Template Chuẩn 4 Nền Tảng — Copy-Paste Ready

> **Cách dùng**: copy template tương ứng nền tảng → thay placeholder `{{...}}` bằng giá trị thật → paste vào URL link đi từ ads. **GA4 sẽ đọc UTM** + **gắn vào Acquisition reports** + **dashboard Looker Studio**.

## 🎯 Vì sao cần UTM chuẩn

Không có UTM:
- GA4 chỉ thấy "facebook / cpc" — không biết campaign nào, ad nào, audience nào.
- Không tách được ROAS theo creative.
- Không A/B test được landing page (creative thắng nhưng LP thua hay LP thắng nhưng creative thua?).

UTM chuẩn:
- Tracker đầy đủ: campaign / ad set / creative / audience.
- Phân tích đa chiều: kênh → campaign → angle → format → audience.
- Gắn với CRM để truy ngược lead/order về exact creative.

## 📋 5 tham số UTM

| Tham số | Bắt buộc | Mô tả |
|---|---|---|
| `utm_source` | ✅ | Nền tảng gốc (meta, google, tiktok, youtube) |
| `utm_medium` | ✅ | Loại media (paid_social, cpc, paid_video) |
| `utm_campaign` | ✅ | Tên campaign (theo naming convention) |
| `utm_content` | ✅ | Phân biệt creative (angle, format, hook, ad ID) |
| `utm_term` | ⚠️ | Audience hoặc keyword (Google Search) |

## 🔵 Template — Meta (Facebook + Instagram)

> Theo Khối 14a dòng 305-306.

```
utm_source=meta
utm_medium=paid_social
utm_campaign={{brand}}_{{objective}}_{{country}}_{{offer}}_{{funnel}}
utm_content={{angle}}_{{format}}_{{hook}}_{{adid}}
utm_term={{audience}}
```

### Ví dụ TPCN

```
utm_source=meta
utm_medium=paid_social
utm_campaign=tpcn_sales_vn_collagen35_bof
utm_content=pain_video_15s_questionhook_120945
utm_term=lal_purchaser_3pct
```

### Placeholder mapping

| Placeholder | Mẫu giá trị |
|---|---|
| `{{brand}}` | tpcn / abchealth / tên brand |
| `{{objective}}` | sales / lead / awareness / engagement |
| `{{country}}` | vn / sg / global |
| `{{offer}}` | collagen35 / vitamin_office / immune_family |
| `{{funnel}}` | tof / mof / bof / rmkt |
| `{{angle}}` | pain / curiosity / proof / offer |
| `{{format}}` | video15s / video30s / carousel / single_image |
| `{{hook}}` | questionhook / numberhook / patternbreak |
| `{{adid}}` | ad ID Meta (số 15-16 chữ số) |
| `{{audience}}` | broad / lal_purchaser_3pct / website30d / ig_engagers365d |

## 🔴 Template — Google Ads

```
utm_source=google
utm_medium=cpc
utm_campaign={{brand}}_{{network}}_{{intent}}_{{offer}}_{{geo}}
utm_content={{adgroup}}_{{rsa_variant}}
utm_term={keyword}
```

### Ví dụ TPCN

```
utm_source=google
utm_medium=cpc
utm_campaign=tpcn_search_nonbrand_collagen_lead_hn
utm_content=collagen_phu_nu_35_rsa1
utm_term={keyword}
```

### Placeholder mapping

| Placeholder | Mẫu giá trị |
|---|---|
| `{{network}}` | search / display / shopping / video / pmax |
| `{{intent}}` | brand / nonbrand |
| `{{geo}}` | hn / hcm / vn |
| `{{adgroup}}` | tên ad group |
| `{{rsa_variant}}` | rsa1 / rsa2 |
| `{keyword}` | **giữ nguyên** — Google tự thay bằng keyword thực tế |

⚠️ **Quan trọng**: với Google, **bật Auto-tagging** (gắn GCLID) song song. UTM bổ sung cho GA4, GCLID dùng cho Google Ads import offline conversion.

## ⚫ Template — TikTok

> Theo Khối 14c dòng 102-103.

```
utm_source=tiktok
utm_medium=paid_social
utm_campaign={{brand}}_{{type}}_{{objective}}_{{offer}}
utm_content={{creative_id}}_{{hook}}_{{format}}
utm_term={{audience}}
```

### Ví dụ TPCN

```
utm_source=tiktok
utm_medium=paid_social
utm_campaign=tpcn_gmvmax_sales_collagen35
utm_content=video01_painhook_demo
utm_term=aud_broad_or_lal_purchase30
```

### Placeholder mapping

| Placeholder | Mẫu giá trị |
|---|---|
| `{{type}}` | gmvmax / live_gmvmax / web_sales |
| `{{objective}}` | sales / awareness / consideration / lead |
| `{{creative_id}}` | video01, spark02, aca03 |
| `{{hook}}` | painhook / curiosityhook / numberhook |
| `{{format}}` | demo / unboxing / step_by_step / reply_to_comment |
| `{{audience}}` | broad / lal_purchase30 / shopactivity_pdp30 |

## 🟢 Template — YouTube (qua Google Ads)

```
utm_source=youtube
utm_medium=paid_video
utm_campaign={{brand}}_{{format}}_{{objective}}_{{offer}}
utm_content={{angle}}_{{video_id}}_{{cta}}
utm_term={{audience}}
```

### Ví dụ TPCN

```
utm_source=youtube
utm_medium=paid_video
utm_campaign=tpcn_skippable_consideration_collagen35
utm_content=expertinterview_yt001_learnmore
utm_term=lal_videoengager30d
```

### Placeholder mapping

| Placeholder | Mẫu giá trị |
|---|---|
| `{{format}}` | skippable / nonskippable / bumper / shorts / infeed / sequence / masthead |
| `{{angle}}` | expertinterview / casestudy / demo / before_after / educational |
| `{{video_id}}` | yt001, yt002... (in-house ID) |
| `{{cta}}` | learnmore / signup / shopnow / watchmore |

## 🚦 6 quy tắc khi đặt UTM

1. **Lowercase + underscore** — KHÔNG dùng dấu cách, viết hoa, ký tự đặc biệt.
   - ❌ `Collagen 35+ Phụ Nữ`
   - ✅ `collagen_phu_nu_35`

2. **Không tiếng Việt có dấu** — GA4 đôi khi encode sai.
   - ❌ `phụ_nữ_35`
   - ✅ `phu_nu_35`

3. **Nhất quán xuyên suốt** — naming convention thống nhất 4 nền tảng + CRM.

4. **Ngắn gọn** — dưới 50 ký tự/tham số (URL không bị truncate).

5. **Document** — lưu naming convention vào Google Sheet master, tất cả người chạy ads dùng cùng.

6. **Không UTM cho organic** — chỉ cho ads/email/affiliate. Organic GA4 tự nhận diện.

## 🛠️ Công cụ hỗ trợ

### URL Builder

- **Google Campaign URL Builder**: https://ga-dev-tools.google/campaign-url-builder/
- **Tự build trong Google Sheet**: cột A-E nhập tham số, cột F = `=CONCATENATE(...)` ra URL hoàn chỉnh.

### QA UTM

- **GA4 Realtime → Source/Medium**: thấy UTM đúng sau 1-2 phút.
- **Tag Assistant** (Chrome extension): debug khi click ad.

## 📊 Đọc UTM trong GA4

| Đường dẫn | Mục đích |
|---|---|
| Acquisition → Traffic acquisition | Tổng quan source/medium |
| Acquisition → User acquisition | Theo dõi user mới |
| Reports → User attributes → Custom report | Xem `utm_campaign`, `utm_content` |
| Explore → Funnel exploration | Phân tích funnel theo campaign/creative |

## 🎯 Hành động cho team ads TPCN

> Đẩy vào [[../../actions|actions.md]].

1. **Chuẩn bị Google Sheet UTM Master** với:
   - Tab 1: Naming convention (placeholder mapping).
   - Tab 2: URL Builder formula.
   - Tab 3: Log UTM đã dùng (tránh trùng).

2. **Tất cả người chạy ads** copy URL từ Sheet — KHÔNG tự gõ tay.

3. **QA UTM** mỗi tuần khi review dashboard:
   - Số campaign trong GA4 = số campaign thực tế.
   - Source/Medium đúng (không có "(not set)" >5%).

4. **Sync với CRM** — khi lead/order về CRM, lưu kèm UTM để truy ngược creative thắng/thua.

## 🔗 Liên quan

- [[Khối 14 - ADS Các nền tảng]]
- [[Checklist QA tracking đa kênh]]
- [[Pixel + CAPI + Event Deduplication]]
