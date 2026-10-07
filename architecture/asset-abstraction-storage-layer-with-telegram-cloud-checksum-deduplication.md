# Asset Abstraction Storage Layer with Telegram Cloud & Checksum Deduplication

**Category:** architecture
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-10-07

## 🔍 Problem / Context
Quản lý lưu trữ tài nguyên số tập trung, chống trùng lặp dữ liệu (Deduplication) và độc lập hoàn toàn giữa CSDL nghiệp vụ với hạ tầng Telegram Cloud Storage.

## 💡 Solution & Implementation
1. Khởi tạo bảng `media_assets` quản lý tập trung toàn bộ metadata tài nguyên theo UUID v4 (SSOT).
2. Dùng SHA-256 hash của binary file để deduplicate trước khi upload.
3. Client và các domain service chỉ lưu và gọi URL bất biến `/api/v1/media/:asset_id`.
4. TelegramStorage sinh Caption JSON có cấu trúc `#INFB_ASSET` cho Disaster Recovery.
5. MediaController proxy stream nhị phân kèm Redis caching 1h và header immutable.

## ⚠️ Anti-Patterns / Pitfalls
Lưu trực tiếp URL thô của Telegram (ví dụ: /api/v1/media/tg/:file_id) vào các bảng CSDL nghiệp vụ (User, Boardgame, Chat, Social) khiến hệ thống bị vendor lock-in và không thể deduplicate hoặc migrate khi chuyển đổi storage provider.

## 📂 Related Files
- `workspace/packages/shared/interface/storage/IMediaAsset.ts`
- `workspace/back-end/src/models/common/MediaAssetModel.ts`
- `workspace/back-end/src/services/infrastructure/TelegramStorage.ts`
- `workspace/back-end/src/services/common/UploadService.ts`
- `workspace/back-end/src/controllers/media/MediaController.ts`

