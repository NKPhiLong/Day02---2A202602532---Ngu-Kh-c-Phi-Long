# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Nguỵ Khắc Phi Long
- Mã học viên: 2A202602532
- Nhóm: Phan Duy Bảo, Nguyễn Anh Tú, Trần Thị Thuý, Nguỵ Khắc Phi Long, Đoàn Duy Bách (5 người)
- Candidate problem nhóm chọn: #1 — Điều phối sự cố bảo trì: khách báo hỏng qua 3 kênh rời rạc (Zalo riêng, gọi điện, nhóm Zalo chung), mọi yêu cầu dồn về một mình quản lý để phân việc cho 2 thợ, không có chỗ ghi nhận tập trung nên thỉnh thoảng có vụ bị trôi và khách phải nhắc lần 2

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tự scan từ 3 bối cảnh thật của mình: sinh viên năm cuối, intern công ty công nghệ, gia sư. Ghi 8 dòng vào bảng scan, phủ đủ 4 lăng kính, mỗi dòng kèm số ước lượng (thời gian/lần × tần suất) | Có 8 candidate để mang vào nhóm, trong đó 3 bài từ bối cảnh intern là bài nhóm ít người có |
| Pitch Problem Card | Pitch 3 candidate từ bối cảnh intern: #10 Onboard codebase (~4 tiếng/module), #11 Điều tra bug từ ticket (~85 phút/ticket × 3 ticket/tuần), #12 Hỏi lại mentor (4-5 lần/tuần). Cố ý chọn 3 bài trải đủ 3 mức Rule / Workflow / Agent | #11 vào shortlist với 29 điểm, đứng thứ 2/3; nhóm dùng #11 làm ví dụ chuẩn cho câu hỏi "khi nào Agent có lý do thật" |
| Challenge bài của bạn khác | Với bài #1 của Bảo, hỏi ngược: "nếu chỉ mình anh được quyền ghi, thì lúc anh bận ai ghi?" Với bài #8 của Thuý, hỏi dữ liệu doanh số có mang ra thử trong lab được không | Câu hỏi thứ nhất làm lộ mâu thuẫn của phương án ban đầu và dẫn tới việc tách quyền ghi nhận khỏi quyền quyết định — chi tiết này đi thẳng vào bản nhóm cuối. Câu thứ hai làm rõ cột "Làm trong lab" của #8 chỉ được 2 điểm |
| Gom trùng / cluster | Tự nhận #10 và #12 của mình trùng pattern với #11 (cụm D) và #14 (cụm A), đề nghị chỉ giữ bài mạnh nhất mỗi cụm thay vì đẩy cả 3 bài vào shortlist | Shortlist gọn còn 3 bài thay vì bị loãng; nhóm không mất thời gian chấm 2 bài cùng gốc |
| Chọn candidate problem | Đồng ý gạt #11 của chính mình sau khi không tách được: trong ~40 phút dò log, bao nhiêu là do ticket mô tả sơ sài (sửa bằng template, không cần AI) và bao nhiêu là do bản chất việc lần log qua nhiều service | Nhóm chốt #1 (30 điểm) thay vì #11 (29 điểm); lý do gạt #11 được ghi nguyên văn vào mục 3.4 làm bằng chứng cho chất lượng quyết định |
| Validation / research | Nhận phần research giải pháp đã có. Đọc tài liệu chính thức của Jira Service Management, AppSheet, TenantCloud/Buildium và Zalo OA API. Cũng nêu ý kiến rằng dòng Interview chưa tính là validation hợp lệ vì người trả lời và người đề xuất bài là cùng một người | Tìm ra chặn lớn nhất của cả bài: Zalo OA API chỉ phủ Official Account, không phủ tin nhắn cá nhân và nhóm chung — tức là giả định "AI đọc luồng Zalo" chưa có đường làm hợp lệ. Phát hiện này làm kết luận Rule / No AI mạnh thêm một bậc, và làm nhóm ghi rõ kế hoạch validation còn thiếu thay vì coi 1 interview là đủ |
| Workflow nhóm | Hỏi để tách bước 2 (ghi nhận) khỏi bước 3 (phân thợ) khi vẽ workflow 6 bước, và đề nghị ghi rõ bằng chứng vì sao khâu thi công không phải bottleneck (thợ luôn nhắn báo lại ngay khi xong) | Bottleneck được khóa vào đúng bước 2 thay vì nói chung chung là "quy trình chậm". Từ đó nhóm viết được tiêu chí phản bác: nếu thợ nói vụ nào cũng tới tay thì bottleneck nằm ở bước 3 và phải vẽ lại workflow |
| Problem Statement | Chất vấn field Boundary của v0 ("chỉ quản lý được ghi và đóng vụ") và đề nghị bỏ câu "sửa chậm làm mất khách, mỗi khách đi mất 1,5-3 triệu" khỏi Impact vì không có bằng chứng | Boundary v1 được sửa thành tách quyền GHI NHẬN khỏi quyền QUYẾT ĐỊNH — đây là thay đổi lớn nhất giữa v0 và v1. Impact v1 tách rõ phần có bằng chứng (giờ công) và bỏ hẳn phần giả định |
| Rule / Workflow / Agent | Ở phần cá nhân: chủ động chọn 3 card trải đủ 3 mức — Onboard codebase (Workflow), Điều tra bug từ log (Agent), Hỏi lại mentor (Rule) — để có cơ sở so sánh mức thay vì mặc định chọn mức cao nhất. *(phần nhóm điền sau Phase 6)* | |
| Decision | Ủng hộ Not Yet thay vì Go: metric đã có cách đo nhưng baseline vẫn là "thi thoảng có vụ bị trôi", chưa phải một con số, trong khi dữ liệu để đếm đã nằm sẵn trong lịch sử chat Zalo | Nhóm chốt Not Yet, kèm việc đếm baseline 2 tuần trước khi quyết Go |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Việc tách quyền ghi nhận khỏi quyền quyết định trong future workflow của nhóm bắt nguồn từ
câu hỏi em đặt ra: nếu chỉ quản lý được ghi thì lúc quản lý bận, vụ vẫn trôi y như cũ.
Ngoài ra, lý do gạt bài #11 của chính em được nhóm giữ nguyên trong mục 3.4 như một ví dụ
về việc không chọn bài chỉ vì nó "có chỗ cho AI".
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Tự nghĩ trước từ 3 bối cảnh của mình, sau đó nhờ AI gợi ý thêm problem theo 4 lăng kính | Mở ra được lăng kính "pain từ người khác" mà em bỏ sót: mentor bị ngắt việc khi em hỏi lại, reviewer phải comment lặp lỗi cũ | Đưa ra hơn 20 gợi ý nhưng nhiều ý em chưa từng trải qua (apply CV, tra log ticket ở quy mô lớn); phần số liệu là AI tự điền ước lượng, không phải số em đo | Bỏ các ý không có trải nghiệm thật, chỉ giữ 8 dòng; đánh dấu rõ số liệu là ước lượng và tự bấm giờ/đếm lại trước khi nộp |
| Problem Card | Nhờ AI đóng vai PM khó tính phản biện từng card | Chỉ ra metric em viết ban đầu ("đề cương tốt hơn", "nhanh hơn") không đo được; chỉ ra em bỏ trống mục non-AI alternative nên trông như đang mặc định phải dùng AI | Gộp 2 bước khác nhau thành một bottleneck; tự suy đoán công ty em dùng Confluence + Slack + ADR trong khi em chưa xác nhận | Tách metric thành thời gian (bấm giờ) + chất lượng (% câu đề cũ được phủ); tách lại bottleneck về đúng 1 bước; kiểm lại công ty thật sự dùng tool nào |
| Workflow | Nhờ AI dựng workflow trước/sau dạng ASCII có thời gian từng bước, boundary và fallback | Nhanh và có sẵn khung để nhìn ra chỗ nào là máy, chỗ nào là AI, chỗ nào là người | Thời gian từng bước ở future state là AI tự chia ra cho đẹp, không dựa trên lần chạy thật nào | Coi các con số future state là giả định cần kiểm, không dùng như kết quả; ghi rõ đây là kỳ vọng chứ không phải đo được |
| Research | Nhờ AI tìm tool/pattern đã giải bài tương tự và tóm tắt họ xử lý bước nào trong workflow | Gợi ra đúng pattern chung của các sản phẩm tốt: máy ghi nhận và nhắc, người vẫn là bên quyết định | Có claim về mức tiết kiệm thời gian nhưng không kèm nguồn kiểm được; một vài tool AI đề xuất thực tế không dùng được vì khách vẫn nhắn qua Zalo | Chỉ giữ link tài liệu chính thức, bỏ toàn bộ số liệu không verify được; loại các tool đòi khách đổi kênh liên lạc |
| Problem Statement | Nhờ AI phản biện 6 field của PS v0, yêu cầu chỉ ra field mơ hồ chứ không viết lại hộ | Chỉ đúng chỗ yếu nhất: baseline "thi thoảng có vụ bị trôi" không phải là số nên metric không chứng minh được cải thiện | AI đề xuất luôn một con số baseline giả định để "cho đủ field" | Không lấy số giả định; giữ nguyên baseline là chưa có và chuyển nó thành điều kiện phải đếm trước khi Go |
| Rule / Workflow / Agent | Nhờ AI so sánh giúp 3 mức trên chính 3 bài của em | Chỉ rõ tiêu chí phân biệt: mơ hồ cao/thấp, phức tạp cao/thấp, và câu hỏi "AI có cần tự quyết bước tiếp theo không" | Ở một lượt em yêu cầu "đổi bài để dùng AI nhiều hơn", AI làm theo và đề xuất bài mới — đây đúng là hướng solution-first mà lab cảnh báo | Tự nhận ra mình đang chọn bài theo độ "ngầu" của giải pháp; đổi hướng thành chọn 3 bài trải đủ 3 mức Rule/Workflow/Agent để chứng minh có tiêu chí chọn mức |
| Decision | Nhờ AI phản biện lựa chọn Rule và hỏi ngược liệu có đang bỏ sót chỗ AI thật sự giúp được | Giúp diễn đạt rõ lập luận loại AI: nếu AI ghi sót một tin báo hỏng thì người phát hiện đầu tiên là khách khi nhắc lần 2 — đúng thứ bài toán sinh ra để diệt | AI vẫn có xu hướng đề xuất thêm một lớp AI "hỗ trợ nhẹ" ở bước ghi nhận dù nhóm đã kết luận Rule là đủ | Giữ nguyên Rule, không thêm AI vào bước ghi nhận; ghi rõ trong bài rằng mức dưới Rule là hiện trạng nên không hạ tiếp được |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.
> Phase Pitch và Challenge: **không dùng AI** — theo quy ước của lab, phần trình bày và phản biện phải bằng hiểu biết của bản thân.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Lúc mới vào lab em cứ nghĩ chọn bài nào cũng được, miễn nghe có vẻ dùng AI được. Đến khi
nghe Thuý trình bày bài chốt doanh số tháng, mất tận 5 ngày mỗi tháng, em mới thấy bài đó
đau hơn hẳn ba bài của em. Nhưng cuối cùng nhóm vẫn không chọn nó, vì chỉ mình Thuý hiểu
nghiệp vụ kế toán, bốn đứa còn lại ngồi nghe mà không biết hỏi gì. Chỗ này em nhớ lâu: bài
đau đến mấy mà cả nhóm không challenge được thì cũng khó làm chặt trong một buổi.

Em cũng tự thấy mình bị solution-first. Ba bài em chuẩn bị lúc đầu toàn dừng ở Rule với
Workflow, em thấy ít AI quá nên định đổi sang bài khác cho hoành tráng hơn, may là nghĩ lại
kịp. Em giữ nguyên ba bài nhưng chọn mỗi bài một mức Rule, Workflow, Agent để còn có cái mà
so với nhau.

Bài điều tra bug từ log là bài em tự tin nhất, vậy mà bị hỏi đúng một câu em trả lời không
được: trong 40 phút dò log thì bao nhiêu phút là do cái ticket viết sơ sài? Nếu phần lớn là
do ticket thì chỉ cần bắt điền form cho đủ là xong, cần gì tới AI. Em ngồi nghĩ một lúc rồi
đồng ý bỏ bài của mình.

Viết Problem Statement thì em thấy metric khó hơn boundary nhiều. Boundary chỉ cần hỏi AI
sai thì ai biết đầu tiên là ra, còn metric thì viết được vài chữ lại quay về nhanh hơn với
gọn hơn. Cuối cùng nhóm phải để Not Yet vì baseline vẫn là thi thoảng có vụ bị trôi, chưa ai
ngồi đếm ra số. Nếu làm lại, em sẽ hỏi số thật là bao nhiêu ngay từ đầu chứ không để đến
cuối mới phát hiện.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI
