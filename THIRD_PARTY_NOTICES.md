# Ghi nguồn dữ liệu bên thứ ba

BBKeyboard dùng các dữ liệu ngôn ngữ sau. App chỉ chứa danh sách từ và số liệu thống kê (tần suất,
xác suất từ đi sau từ) dựng từ các nguồn này, không chứa văn bản gốc.

| Dữ liệu | Dùng cho | Giấy phép |
|---|---|---|
| [FrequencyWords](https://github.com/hermitdave/FrequencyWords) — Hermit Dave | Từ điển tiếng Việt và tiếng Anh (`dict_vi.txt`, `dict_en.txt`) | CC BY-SA 4.0 |
| [OpenSubtitles v2018](https://opus.nlpl.eu/OpenSubtitles/corpus/version/OpenSubtitles) qua OPUS — P. Lison & J. Tiedemann, 2016 | Mô hình đoán từ (văn nói) | Theo điều khoản của OPUS / opensubtitles.org |
| [TED2020](https://opus.nlpl.eu/TED2020/corpus/version/TED2020) — N. Reimers & I. Gurevych, 2020 | Mô hình đoán từ | CC BY-NC-ND 4.0 (chỉ dùng phi thương mại) |
| [CCAligned](https://opus.nlpl.eu/CCAligned/corpus/version/CCAligned), [CCMatrix](https://opus.nlpl.eu/CCMatrix/corpus/version/CCMatrix) qua OPUS (dựa trên Common Crawl) | Mô hình đoán từ (văn bản web) | Theo điều khoản của OPUS / Common Crawl |
| [Tatoeba](https://tatoeba.org) qua OPUS | Mô hình đoán từ (câu hội thoại) | CC BY 2.0 FR |
| [Leipzig Corpora Collection](https://wortschatz.uni-leipzig.de) — vie_news_2022_300K, Universität Leipzig | Mô hình đoán từ (tin tức) | CC BY 4.0 |

Vì có dữ liệu TED2020 (phi thương mại), BBKeyboard được phát hành miễn phí. Nếu muốn phát hành có thu
phí, cần dựng lại mô hình không dùng TED2020 (`tools/build_lm.js`).
