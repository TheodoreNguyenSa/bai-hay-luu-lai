# Bài hay lưu lại

Tuyển tập các repo và công cụ hay về AI agent, coding agent và công cụ cho developer. Mỗi mục chỉ nêu repo/link chính thức và công dụng.

## 1. ARTEMIS — AI agent điều khiển điện thoại Android
- Repo: https://github.com/google/artemis
- Công dụng: điều khiển điện thoại Android thật hoặc emulator như người dùng — mở app, bấm, gõ, kiểm tra kết quả, chuyển app, thu thập screenshot và Logcat. Chạy qua web, CLI, Python và MCP cho các coding agent phổ biến. Cần máy Android bật USB debugging hoặc emulator, Python 3.12+ và API key model đa phương thức.

## 2. Browsentic — AI dùng luôn trình duyệt thật đã đăng nhập
- Repo: https://github.com/imshaikot/browsentic
- Công dụng: điều khiển trình duyệt thật đã đăng nhập (Chrome, Edge, Brave, Arc, Firefox) qua extension + Bridge local, dùng luôn session đã login thay vì profile trắng. Chạy bằng agent CLI đã có, không cần API key riêng, với 52 page tool: điều hướng, đọc file, upload/download, giọng nói, chỉ tay vào màn hình.

## 3. Maximizing Value from Claude Code — hướng dẫn của Anthropic
- Link: https://anthropic.ondemand.goldcast.io/on-demand/5ca27c0b-2eab-45d5-bded-b18e6a2f0d7c
- Công dụng: hướng dẫn dùng Claude Code sao cho rẻ và hiệu quả hơn — token, cấu trúc request, mô hình giá, cache optimization, chọn model, tối ưu context, cấu hình effort, sub-agent và cài đặt cho admin.

## 4. Chorus — gom Claude Code, Codex, Antigravity vào một cửa sổ
- Link: https://chorus-cli.web.app/
- Công dụng: chạy trực tiếp 3 CLI gốc `claude`, `codex`, `agy` trong một cửa sổ, giữ nguyên slash command, plugin, MCP, file CLAUDE.md/AGENTS.md và login + gói riêng của từng CLI. Bộ nhớ chung qua Chorus MCP server, handoff 1 click giữa các agent, approvals gom về 1 inbox, 1 thư viện skill chung link vào mọi agent. Chạy trên macOS Apple silicon và Linux; Windows chỉ qua WSL.

## 5. GoodAIList — các repo AI nổi bật
Nguồn: bảng GoodAIList của Chip Huyen, cập nhật hàng ngày.

### 5.1 morluto/rea — Reverse Engineer Anything
- Repo: https://github.com/morluto/rea
- Công dụng: MCP server + CLI cho coding agent dùng các tool reverse engineering sẵn có (Ghidra, IDA Pro, Hopper, JADX cho Android, Binwalk/Unblob cho firmware), trả về pseudocode, module graph, execution trace kèm evidence và giới hạn. Chỉ dùng cho nghiên cứu hợp pháp, giáo dục, tương thích và phân tích phần mềm mình sở hữu.

### 5.2 Gathin23/cleanyourtv — dọn Android TV
- Repo: https://github.com/Gathin23/cleanyourtv
- Công dụng: debloat Android TV / Google TV qua Wi-Fi bằng ADB, không root, chỉ `pm disable-user` (không uninstall, khôi phục được bằng restore script), kèm launcher nhẹ kiểu Apple TV.

### 5.3 Zagitta/gpu-unlock — mở khóa FP/BF16 cho Nvidia dòng 3000
- Repo: https://github.com/Zagitta/gpu-unlock
- Công dụng: Linux kernel module, chạy trước khi driver Nvidia bind, mở tốc độ issue FP/BF16 FMA lên mức card chuyên nghiệp cho chip GA102/GA103/GA104/GA106 (3060 12GB → 3090 Ti). Không cần flash vBIOS, không patch driver.

### 5.4 debpalash/VoiceStudio — thay ElevenLabs, chạy local, clone giọng
- Repo: https://github.com/debpalash/VoiceStudio
- Công dụng: app desktop Electron + Python backend, clone giọng, design giọng, dictation, transcription, audiobook, local API + MCP cho agent. Engine mặc định OmniVoice.

### 5.5 Nutlope/hallmark — skill chống "AI slop" khi thiết kế
- Repo: https://github.com/Nutlope/hallmark
- Công dụng: skill cho Claude Code, Codex, Cursor, OpenCode — chọn theme từ catalog, chạy linter trong trình duyệt thật để soi các dấu hiệu "nhìn là biết AI làm", rồi reviewer ở context mới chốt lần cuối.

### 5.6 cloudflare/security-audit-skill — audit bảo mật nhiều giai đoạn
- Repo: https://github.com/cloudflare/security-audit-skill
- Công dụng: skill biến coding agent thành auditor, chạy 6 phase với adversarial validation — agent kiểm tra finding không phải agent tìm ra finding đó. Bao phủ web/auth, client, cloud/deploy, supply chain/CI, RPC/messaging, data isolation, native/mobile, và AI/LLM (prompt injection, agent tools).

### 5.7 AgriciDaniel/claude-seo — skill SEO cho Claude Code
- Repo: https://github.com/AgriciDaniel/claude-seo
- Công dụng: plugin Claude Code, 26 sub-skill + 19 sub-agent, 34 command — audit SEO kỹ thuật, E-E-A-T, schema, GEO/AEO, local SEO, backlink, keyword cluster, llms.txt, WebMCP.

## 6. Tongyi-MAI/OpenGCUA — stack mở cho computer-use agent
- Repo: https://github.com/Tongyi-MAI/OpenGCUA
- Paper: https://arxiv.org/abs/2610.22200
- Công dụng: stack mở cho generalist computer-use agent — agent tự chọn cách quan sát và hành động: đọc accessibility tree, gọi API của app, chạy shell, hoặc viết chương trình Python gộp GUI + shell + API trong một lần chạy (có vòng lặp, rẽ nhánh, kết quả trung gian). Kèm ví dụ tích hợp OSWorld, evaluation trajectories của 8 model frontier, harness macOS real-device và Cross-Device SDK.

## 7. StykAnimate — app animation người que miễn phí, open source GPL-3.0
- Web: https://app.stykanimate.com
- Tải: https://stykanimate.com
- Source: https://github.com/filippocalippo/stykanimate-app
- Công dụng: app animation người que cho Windows, Linux và trình duyệt, successor hiện đại của Pivot Animator, mở được file Pivot (.piv, .stk) và Stick Nodes. Pose figure bằng IK tay/chân, timeline Simple và Advanced (layers, folders, keys, easing), camera follow, particle effects, motion paths, onion skins. Export MP4 (preset YouTube/Shorts/TikTok), WebM trong suốt, GIF, APNG và frames. Chạy hoàn toàn local.

## 8. Agency Agents — cả công ty AI trong 1 repo
- Repo: https://github.com/msitarzewski/agency-agents
- Công dụng: mỗi agent là 1 file Markdown (tên, mô tả, vai trò, tính cách, workflow, deliverable, success metrics), tổ chức theo division: Engineering, Design, Marketing, Sales, Product, Finance, Game Development, Security, Support, Healthcare, GIS, AR/VR và nhiều division khác. Cài đúng team mình cần vào Claude Code, Cursor, Copilot, Codex, Gemini CLI, Antigravity, OpenCode... qua script install hoặc app desktop.

## 9. Agent-Reach ("mắt") + Browser MCP ("tay") cho AI agent
- Agent-Reach: https://github.com/Panniantong/Agent-Reach
- Công dụng của Agent-Reach: CLI chỉ đọc, cho agent đọc và tìm trên X, Reddit, YouTube, GitHub, Bilibili, Xiaohongshu, LinkedIn... mà không cần API trả phí, mỗi platform có danh sách tool ưu tiên + dự phòng tự đổi khi hỏng. Chỉ đọc, không đăng, không comment, không like.
- Công dụng của Browser MCP: điều khiển trình duyệt thật để làm mọi thao tác web — linh hoạt hơn Agent-Reach nhưng chậm hơn và tốn token hơn. Lưu ý: có nhiều project cùng tên Browser MCP, phải xác định đúng extension ID / repo trước khi dùng và chỉ thử trên profile phụ.

## 10. Anatomy — skill Claude Code vẽ "máy giải thích khái niệm" bằng hình isometric tương tác
- Repo: https://github.com/wheresryan22/anatomy
- Công dụng: agent skill cho Claude Code (cũng chạy Antigravity, OpenCode, Codex, MiniMax Code) — hỏi 1 khái niệm kỹ thuật, nó "phát minh" 1 vật thể vật lý mà cách hoạt động của vật đó chính là khái niệm (ví dụ cache thành ổ khóa pin-tumbler). Output là SVG isometric chi tiết trong card có tiêu đề + hint + live readout, tương tác bằng chuột/bàn phím, xuất được standalone HTML, file .svg độc lập hoặc component React/Next.js. Chỉ vẽ máy móc, dụng cụ, đồ nội thất — không vẽ người, không vẽ bản đồ chính xác, không phải thư viện chart.

## 11. Impeccable — "từ vựng thiết kế" chống AI slop cho coding agent
- Repo: https://github.com/pbakaus/impeccable
- Công dụng: skill thiết kế cho AI coding agent với 24 lệnh dùng chung 1 từ vựng với AI (`init` ghi PRODUCT.md, rồi `audit`, `critique`, `polish`, `bolder`, `quieter`, `distill`...) cộng 62 rule detector xác định chạy local không cần LLM hay API key, bắt các lỗi như gradient tím, bounce easing, dark glow, line quá dài, touch target nhỏ. Hook design chạy detector mỗi khi lưu file UI, Live Mode thử biến thể visual trực tiếp trong trình duyệt cho project local.

## 12. Nextcloud Server — cloud tự host, mã nguồn mở
- Repo: https://github.com/nextcloud/server
- Công dụng: lưu trữ file, contacts, calendars trên server do mình chọn thay vì cloud thương mại, đồng bộ dữ liệu giữa các thiết bị, chia sẻ và cộng tác với người khác, mở rộng bằng hàng trăm app (Calendar, Contacts, Mail, Video Chat...). Bảo mật bằng cơ chế mã hóa và xác thực 2 yếu tố.

## 13. Stock Market Signal Automation — tự động hoá tín hiệu swing-trade
- Repo: https://github.com/cporter202/stock-market-signal-automation
- Công dụng: hướng dẫn + ví dụ phía người dùng cho hệ thống tín hiệu cổ phiếu KamdenAI — nhận signal event qua signed webhook, kiểm chứng chữ ký, rồi đẩy vào dashboard, alerts, Google Sheets, Discord và AI agent của riêng mình. Kèm ví dụ receiver Node/Python, Discord formatter, AI prompt builder, risk sizing calculator và dashboard xem trước. Lưu ý: engine chọn tín hiệu không nằm trong repo (repo chỉ có guide và ví dụ), các ví dụ dùng mã và giá giả lập, và hệ thống không đặt lệnh tại broker — người dùng tự thực thi.

## 14. Logo Design Skill — quy trình thiết kế logo đóng gói thành agent skill
- Repo: https://github.com/kaankiziltug/logo-design-skill
- Công dụng: biến Claude, Gemini CLI, Codex và các agent hỗ trợ Agent Skills thành designer nhận diện có kỷ luật — từ brief, nghiên cứu, lên 8–12 ý tưởng, dựng 3 concept bằng SVG, kiểm tra (audit, test 16 px, 1 màu, trên kệ đối thủ), tới điểm dừng để người dùng chọn hướng rồi mới làm bộ kit (màu, lockups, board trình bày, favicon/app-icon, guidelines). Kèm thư viện tham chiếu 1.400+ logo SVG có thật (để học cấu trúc và tránh trùng lặp, không sao chép) và bộ tool Python không cần dependency để audit SVG, làm test sheet, board trình bày, render PNG và export bộ favicon/app-icon/web-manifest.

## 15. Bộ 18 repo làm video bằng code — chia 6 "phòng ban"
### Phòng 01 — Teacher (dạy agent)
- https://github.com/remotion-dev/skills — Công dụng: Agent Skills chính thức của Remotion, dạy coding agent best practices làm video bằng Remotion (tạo project, viết markup, render, phụ đề, bản đồ, SaaS).
- https://github.com/greensock/gsap-skills — Công dụng: Agent Skills chính thức của GSAP, dạy coding agent dùng GSAP đúng cách (core animation, timeline, ScrollTrigger, plugin, hiệu năng).
### Phòng 02 — Artist (hình ảnh)
- https://github.com/svg/svgo — Công dụng: tối ưu file SVG, giảm dung lượng và dọn metadata không cần thiết.
- https://github.com/vercel/satori — Công dụng: chuyển HTML/CSS thành SVG (rồi sang PNG), dùng để tạo hình ảnh và thumbnail theo dữ liệu.
### Phòng 03 — Animation (chuyển động)
- https://github.com/greensock/GSAP — Công dụng: thư viện animation JavaScript chính, timeline và easing, đóng vai "nhạc trưởng" cho chuyển động.
- https://github.com/juliangarnier/anime — Công dụng: animation engine JavaScript nhẹ, mạnh cho vẽ SVG và hiệu ứng nét vẽ.
- https://github.com/motiondivision/motion — Công dụng: thư viện animation cho React (trước đây là Framer Motion), tương tác và gesture cho UI.
- https://github.com/LottieFiles/dotlottie-web — Công dụng: player chính thức để phát animation Lottie và dotLottie trên web.
### Phòng 04 — Editing Room (dựng phim)
- https://github.com/remotion-dev/remotion — Công dụng: framework làm video bằng React, render ra MP4, là "editor" chính.
- https://github.com/motion-canvas/motion-canvas — Công dụng: làm video giảng dạy / explainer bằng code TypeScript.
### Phòng 05 — 3D Filming (quay 3D)
- https://github.com/mrdoob/three.js — Công dụng: thư viện 3D WebGL nền tảng để dựng cảnh 3D.
- https://github.com/pmndrs/react-three-fiber — Công dụng: renderer React cho Three.js, dựng cảnh 3D bằng component.
- https://github.com/pmndrs/drei — Công dụng: bộ helper cho React Three Fiber (camera, controls, lights, environment...).
- https://github.com/dimforge/rapier.js — Công dụng: engine vật lý cho cảnh 3D (bản JavaScript của Rapier).
- https://github.com/pmndrs/postprocessing — Công dụng: hiệu ứng hậu kỳ cho Three.js / React Three Fiber (bloom, depth of field, vignette...).
### Phòng 06 — Sound & Post (âm thanh + hậu kỳ)
- https://github.com/goldfire/howler.js — Công dụng: thư viện âm thanh cho web, phát và điều khiển audio, hỗ trợ spatial audio.
- https://github.com/Vanilagy/mediabunny — Công dụng: thư viện xử lý multimedia ngay trong trình duyệt (đọc, ghi, đóng gói MP4/WebM...).
- https://github.com/FFmpeg/FFmpeg — Công dụng: encode và chuyển đổi video/audio, bước xuất file cuối cùng.

## 16. FULL ROADMAP AI AGENT (Từ A–Z) — lộ trình học AI Agent cho người mới
- https://docs.google.com/document/d/18WVsWb3I6v_5RGTnkmbbXjMIn7PsSE8CQ7KxkNo2H08/edit?usp=sharing — Công dụng: tài liệu tổng hợp lộ trình học AI Agent gồm 8 video nhập môn và chuyên sâu, 10 repo GitHub thực hành, 5 tài liệu hướng dẫn chính hãng (Google, Anthropic, OpenAI), 7 cuốn sách và 4 bài nghiên cứu nền tảng (ReAct, Generative Agents, Toolformer, Chain-of-Thought).
