# UET Beamer Theme

Template Beamer cho Trường Đại học Công nghệ -- ĐHQGHN (VNU-UET).

Theme được adapt từ [HUST-Beamer-Theme](https://github.com/ndgnuh/HUST-Beamer-Theme) (cảm ơn tác giả [ndgnuh](https://github.com/ndgnuh)).

Xem slide mẫu:
- [Slide UET (16:9)](example_uet.pdf)
- [Slide UET (4:3)](example_uet_43.pdf)

## Cách dùng

Copy các file `*.sty` và thư mục `res` vào project LaTeX của bạn.

```latex
\documentclass[aspectratio=169, 11pt]{beamer}
\usetheme{uet}
```

Các lệnh tùy chọn:
- `\slogan{<text>}`: Đặt khẩu hiệu chân trang bìa (mặc định: `SÁNG TẠO -- TIÊN PHONG -- CHẤT LƯỢNG CAO`).
- `\schoollogo{<đường_dẫn_ảnh>}`: Thêm logo khoa / viện bên cạnh logo trường.
- `\thankpage[<lời_cảm_ơn>]`: Tạo nội dung cho slide kết thúc (`\begin{frame}[noframenumbering,Thank] \thankpage \end{frame}`).

## Biên dịch

```shell
xelatex example_uet.tex
bibtex example_uet
xelatex example_uet.tex
xelatex example_uet.tex
```
