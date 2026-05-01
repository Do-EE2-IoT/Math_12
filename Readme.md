# Bảng công thức giới hạn, đạo hàm và nguyên hàm

Tài liệu tổng hợp từ các ảnh trong thư mục [`images`](./images), trình bày lại theo định dạng Markdown để dễ đọc, dễ tra cứu và hiển thị tốt trên GitHub.

## Mục lục

- [Bảng giới hạn thường dùng](#bảng-giới-hạn-thường-dùng)
- [Quy tắc đạo hàm cơ bản](#quy-tắc-đạo-hàm-cơ-bản)
- [Bảng đạo hàm hàm số sơ cấp](#bảng-đạo-hàm-hàm-số-sơ-cấp)
- [Đạo hàm hàm lượng giác](#đạo-hàm-hàm-lượng-giác)
- [Đạo hàm hàm lượng giác ngược](#đạo-hàm-hàm-lượng-giác-ngược)
- [Đạo hàm phân thức thường gặp](#đạo-hàm-phân-thức-thường-gặp)
- [Đạo hàm cấp cao](#đạo-hàm-cấp-cao)
- [Bảng nguyên hàm cơ bản](#bảng-nguyên-hàm-cơ-bản)
- [Nguyên hàm có hàm hợp tuyến tính](#nguyên-hàm-có-hàm-hợp-tuyến-tính)

## Quy ước

Trong các công thức dưới đây:

- \(u = u(x)\), \(v = v(x)\) là các hàm số khả vi.
- \(k, a, b, c, d, m, n\) là hằng số; các mẫu số được giả sử khác \(0\).
- \(C\) là hằng số tích phân.
- Với \(\log_a x\), điều kiện mặc định là \(a > 0, a \ne 1, x > 0\).

## Bảng giới hạn thường dùng

### Quy tắc tính giới hạn

Giả sử \(\lim\limits_{x \to x_0} f(x) = A\), \(\lim\limits_{x \to x_0} g(x) = B\).

| Biểu thức | Giới hạn |
|---|---:|
| \(\lim\limits_{x \to x_0}[f(x) + g(x)]\) | \(A + B\) |
| \(\lim\limits_{x \to x_0}[f(x) - g(x)]\) | \(A - B\) |
| \(\lim\limits_{x \to x_0} kf(x)\) | \(kA\) |
| \(\lim\limits_{x \to x_0} f(x)g(x)\) | \(AB\) |
| \(\lim\limits_{x \to x_0}\dfrac{f(x)}{g(x)}\) | \(\dfrac{A}{B}\), nếu \(B \ne 0\) |
| \(\lim\limits_{x \to x_0}[f(x)]^n\) | \(A^n\) |
| \(\lim\limits_{x \to x_0}\sqrt[n]{f(x)}\) | \(\sqrt[n]{A}\), nếu biểu thức xác định |

### Giới hạn cơ bản khi \(x \to 0\)

| Công thức | Kết quả |
|---|---:|
| \(\lim\limits_{x \to 0}\dfrac{\sin x}{x}\) | \(1\) |
| \(\lim\limits_{x \to 0}\dfrac{\tan x}{x}\) | \(1\) |
| \(\lim\limits_{x \to 0}\dfrac{x}{\sin x}\) | \(1\) |
| \(\lim\limits_{x \to 0}\dfrac{x}{\tan x}\) | \(1\) |
| \(\lim\limits_{x \to 0}\dfrac{1 - \cos x}{x^2}\) | \(\dfrac{1}{2}\) |
| \(\lim\limits_{x \to 0}\dfrac{\cos x - 1}{x^2}\) | \(-\dfrac{1}{2}\) |
| \(\lim\limits_{x \to 0}\dfrac{\arcsin x}{x}\) | \(1\) |
| \(\lim\limits_{x \to 0}\dfrac{\arctan x}{x}\) | \(1\) |

### Giới hạn mũ, logarit và số \(e\)

| Công thức | Kết quả |
|---|---:|
| \(\lim\limits_{x \to 0}\dfrac{e^x - 1}{x}\) | \(1\) |
| \(\lim\limits_{x \to 0}\dfrac{a^x - 1}{x}\) | \(\ln a\) |
| \(\lim\limits_{x \to 0}\dfrac{\ln(1 + x)}{x}\) | \(1\) |
| \(\lim\limits_{x \to 0}\dfrac{\log_a(1 + x)}{x}\) | \(\dfrac{1}{\ln a}\) |
| \(\lim\limits_{x \to 0}(1 + x)^{1/x}\) | \(e\) |
| \(\lim\limits_{x \to \infty}\left(1 + \dfrac{1}{x}\right)^x\) | \(e\) |
| \(\lim\limits_{x \to \infty}\left(1 + \dfrac{k}{x}\right)^x\) | \(e^k\) |
| \(\lim\limits_{x \to 0}\dfrac{(1 + x)^\alpha - 1}{x}\) | \(\alpha\) |

### Giới hạn vô cực và so sánh bậc

| Công thức | Kết quả |
|---|---:|
| \(\lim\limits_{x \to \infty}\dfrac{1}{x^\alpha}\), \(\alpha > 0\) | \(0\) |
| \(\lim\limits_{x \to \infty}\dfrac{\ln x}{x^\alpha}\), \(\alpha > 0\) | \(0\) |
| \(\lim\limits_{x \to \infty}\dfrac{x^\alpha}{a^x}\), \(a > 1,\ \alpha > 0\) | \(0\) |
| \(\lim\limits_{x \to \infty}\dfrac{a^x}{x^\alpha}\), \(a > 1,\ \alpha > 0\) | \(+\infty\) |
| \(\lim\limits_{x \to \infty}\dfrac{a_nx^n + a_{n-1}x^{n-1} + \cdots + a_0}{b_mx^m + b_{m-1}x^{m-1} + \cdots + b_0}\) | So sánh bậc \(n\) và \(m\) |

Với phân thức hữu tỉ khi \(x \to \infty\):

| Trường hợp | Kết quả |
|---|---:|
| \(n < m\) | \(0\) |
| \(n = m\) | \(\dfrac{a_n}{b_m}\) |
| \(n > m\) | \(\pm\infty\) hoặc không tồn tại hữu hạn, tùy dấu và bậc |

### Các dạng vô định thường gặp

| Dạng vô định | Cách xử lý hay dùng |
|---|---|
| \(\dfrac{0}{0}\) | Phân tích nhân tử, rút gọn, nhân liên hợp, dùng giới hạn cơ bản |
| \(\dfrac{\infty}{\infty}\) | Chia cho lũy thừa bậc cao nhất hoặc so sánh tốc độ tăng |
| \(0\cdot\infty\) | Biến đổi về dạng \(\dfrac{0}{0}\) hoặc \(\dfrac{\infty}{\infty}\) |
| \(\infty - \infty\) | Quy đồng, nhân liên hợp hoặc biến đổi biểu thức |
| \(1^\infty,\ 0^0,\ \infty^0\) | Đặt \(y = f(x)^{g(x)}\), lấy \(\ln y = g(x)\ln f(x)\) |

## Quy tắc đạo hàm cơ bản

| Dạng hàm | Đạo hàm |
|---|---:|
| \((u + v)'\) | \(u' + v'\) |
| \((u - v)'\) | \(u' - v'\) |
| \((ku)'\) | \(ku'\) |
| \((uv)'\) | \(u'v + uv'\) |
| \(\left(\dfrac{u}{v}\right)'\) | \(\dfrac{u'v - uv'}{v^2}\) |
| \(\left(\dfrac{1}{v}\right)'\) | \(-\dfrac{v'}{v^2}\) |
| \(\left(\dfrac{k}{u}\right)'\) | \(-\dfrac{ku'}{u^2}\) |

## Bảng đạo hàm hàm số sơ cấp

| Hàm số theo \(x\) | Đạo hàm | Hàm hợp \(u = u(x)\) | Đạo hàm hàm hợp |
|---|---:|---|---:|
| \(kx\) | \(k\) | \(ku\) | \(ku'\) |
| \(x^n\) | \(nx^{n-1}\) | \(u^n\) | \(nu^{n-1}u'\) |
| \(\dfrac{1}{x}\) | \(-\dfrac{1}{x^2}\) | \(\dfrac{1}{u}\) | \(-\dfrac{u'}{u^2}\) |
| \(\sqrt{x}\) | \(\dfrac{1}{2\sqrt{x}}\) | \(\sqrt{u}\) | \(\dfrac{u'}{2\sqrt{u}}\) |
| \(e^x\) | \(e^x\) | \(e^u\) | \(u'e^u\) |
| \(a^x\) | \(a^x\ln a\) | \(a^u\) | \(u'a^u\ln a\) |
| \(\ln x\) | \(\dfrac{1}{x}\) | \(\ln u\) | \(\dfrac{u'}{u}\) |
| \(\log_a x\) | \(\dfrac{1}{x\ln a}\) | \(\log_a u\) | \(\dfrac{u'}{u\ln a}\) |

## Đạo hàm hàm lượng giác

| Hàm số | Đạo hàm | Ghi chú tương đương |
|---|---:|---|
| \(\sin x\) | \(\cos x\) |  |
| \(\cos x\) | \(-\sin x\) |  |
| \(\tan x\) | \(\dfrac{1}{\cos^2 x}\) | \(1 + \tan^2 x = \sec^2 x\) |
| \(\cot x\) | \(-\dfrac{1}{\sin^2 x}\) | \(-(1 + \cot^2 x) = -\csc^2 x\) |
| \(\sec x\) | \(\sec x\tan x\) |  |
| \(\csc x\) | \(-\csc x\cot x\) |  |

### Hàm hợp lượng giác

| Hàm hợp | Đạo hàm |
|---|---:|
| \(\sin u\) | \(u'\cos u\) |
| \(\cos u\) | \(-u'\sin u\) |
| \(\tan u\) | \(\dfrac{u'}{\cos^2 u} = u'(1 + \tan^2 u)\) |
| \(\cot u\) | \(-\dfrac{u'}{\sin^2 u} = -u'(1 + \cot^2 u)\) |
| \(\sec u\) | \(u'\sec u\tan u\) |
| \(\csc u\) | \(-u'\csc u\cot u\) |

## Đạo hàm hàm lượng giác ngược

| Hàm số | Đạo hàm | Điều kiện thường dùng |
|---|---:|---|
| \(\arcsin x\) | \(\dfrac{1}{\sqrt{1 - x^2}}\) | \(-1 < x < 1\) |
| \(\arccos x\) | \(-\dfrac{1}{\sqrt{1 - x^2}}\) | \(-1 < x < 1\) |
| \(\arctan x\) | \(\dfrac{1}{1 + x^2}\) | \(x \in \mathbb{R}\) |
| \(\arccot x\) | \(-\dfrac{1}{1 + x^2}\) | \(x \in \mathbb{R}\) |

## Đạo hàm phân thức thường gặp

| Dạng hàm | Đạo hàm | Điều kiện |
|---|---:|---|
| \(\dfrac{ax + b}{cx + d}\) | \(\dfrac{ad - bc}{(cx + d)^2}\) | \(c \ne 0,\ ad - bc \ne 0,\ cx + d \ne 0\) |
| \(\dfrac{ax^2 + bx + c}{a'x + b'}\) | \(\dfrac{aa'x^2 + 2ab'x + bb' - a'c}{(a'x + b')^2}\) | \(aa' \ne 0,\ a'x + b' \ne 0\) |
| \(\dfrac{ax^2 + bx + c}{a_1x^2 + b_1x + c_1}\) | \(\dfrac{\begin{vmatrix}a&b\\a_1&b_1\end{vmatrix}x^2 + 2\begin{vmatrix}a&c\\a_1&c_1\end{vmatrix}x + \begin{vmatrix}b&c\\b_1&c_1\end{vmatrix}}{(a_1x^2 + b_1x + c_1)^2}\) | \(a_1x^2 + b_1x + c_1 \ne 0\) |

## Đạo hàm cấp cao

| Hàm số | Đạo hàm cấp \(n\) |
|---|---:|
| \(x^m\), với \(m \ge n\) | \((x^m)^{(n)} = m(m - 1)(m - 2)\cdots(m - n + 1)x^{m-n}\) |
| \(x^m\), với \(m < n\) | \((x^m)^{(n)} = 0\) |
| \(\log_a x\) | \((\log_a x)^{(n)} = (-1)^{n-1}\dfrac{(n-1)!}{\ln a}\cdot\dfrac{1}{x^n}\) |
| \(\ln x\) | \((\ln x)^{(n)} = (-1)^{n-1}(n-1)!x^{-n}\) |
| \(e^{kx}\) | \((e^{kx})^{(n)} = k^n e^{kx}\) |
| \(\dfrac{1}{ax + b}\) | \(\left(\dfrac{1}{ax + b}\right)^{(n)} = (-1)^n a^n n!\dfrac{1}{(ax + b)^{n+1}}\) |
| \(a^x\) | \((a^x)^{(n)} = (\ln a)^n a^x\) |
| \(\sin ax\) | \((\sin ax)^{(n)} = a^n\sin\left(ax + n\dfrac{\pi}{2}\right)\) |
| \(\cos ax\) | \((\cos ax)^{(n)} = a^n\cos\left(ax + n\dfrac{\pi}{2}\right)\) |

## Bảng nguyên hàm cơ bản

| Hàm số dưới dấu tích phân | Nguyên hàm |
|---|---:|
| \(x^\alpha\), \(\alpha \ne -1\) | \(\displaystyle\int x^\alpha\,dx = \dfrac{x^{\alpha+1}}{\alpha+1} + C\) |
| \(\dfrac{1}{x}\) | \(\displaystyle\int \dfrac{1}{x}\,dx = \ln\lvert x\rvert + C\) |
| \(e^x\) | \(\displaystyle\int e^x\,dx = e^x + C\) |
| \(a^x\) | \(\displaystyle\int a^x\,dx = \dfrac{a^x}{\ln a} + C\) |
| \(\sin x\) | \(\displaystyle\int \sin x\,dx = -\cos x + C\) |
| \(\cos x\) | \(\displaystyle\int \cos x\,dx = \sin x + C\) |
| \(\dfrac{1}{\cos^2 x}\) | \(\displaystyle\int \dfrac{1}{\cos^2 x}\,dx = \tan x + C\) |
| \(\dfrac{1}{\sin^2 x}\) | \(\displaystyle\int \dfrac{1}{\sin^2 x}\,dx = -\cot x + C\) |
| \(\sec x\tan x\) | \(\displaystyle\int \sec x\tan x\,dx = \sec x + C\) |
| \(\csc x\cot x\) | \(\displaystyle\int \csc x\cot x\,dx = -\csc x + C\) |

## Nguyên hàm có hàm hợp tuyến tính

| Hàm số dưới dấu tích phân | Nguyên hàm |
|---|---:|
| \((ax + b)^\alpha\), \(\alpha \ne -1\) | \(\displaystyle\int (ax + b)^\alpha\,dx = \dfrac{(ax + b)^{\alpha+1}}{a(\alpha+1)} + C\) |
| \(\dfrac{1}{ax + b}\) | \(\displaystyle\int \dfrac{1}{ax + b}\,dx = \dfrac{1}{a}\ln\lvert ax + b\rvert + C\) |
| \(e^{ax+b}\) | \(\displaystyle\int e^{ax+b}\,dx = \dfrac{1}{a}e^{ax+b} + C\) |
| \(a^{kx+b}\) | \(\displaystyle\int a^{kx+b}\,dx = \dfrac{a^{kx+b}}{k\ln a} + C\) |
| \(\sin(ax + b)\) | \(\displaystyle\int \sin(ax + b)\,dx = -\dfrac{1}{a}\cos(ax + b) + C\) |
| \(\cos(ax + b)\) | \(\displaystyle\int \cos(ax + b)\,dx = \dfrac{1}{a}\sin(ax + b) + C\) |
| \(\dfrac{1}{\cos^2(ax + b)}\) | \(\displaystyle\int \dfrac{1}{\cos^2(ax + b)}\,dx = \dfrac{1}{a}\tan(ax + b) + C\) |
| \(\dfrac{1}{\sin^2(ax + b)}\) | \(\displaystyle\int \dfrac{1}{\sin^2(ax + b)}\,dx = -\dfrac{1}{a}\cot(ax + b) + C\) |

## Nguồn ảnh

- [`dao_ham_chung.png`](./images/dao_ham_chung.png)
- [`dao_ham_so_cap.png`](./images/dao_ham_so_cap.png)
- [`dao_ham_luong_giac.png`](./images/dao_ham_luong_giac.png)
- [`dao_ham_phan_thuc.png`](./images/dao_ham_phan_thuc.png)
- [`dao_ham_cap_cao.png`](./images/dao_ham_cap_cao.png)
- [`nguyen_ham.png`](./images/nguyen_ham.png)

## Ghi chú nhanh

- Đạo hàm của hàm hợp luôn nhân thêm đạo hàm bên trong, ví dụ \((f(u))' = f'(u)u'\).
- Nguyên hàm của hàm hợp tuyến tính \(f(ax+b)\) thường chia thêm cho hệ số \(a\).
- Khi dùng công thức logarit và lũy thừa, cần kiểm tra điều kiện xác định của hàm số trước khi áp dụng.
