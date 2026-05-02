# Toán 12 Core - Công thức và cách dùng nhanh

Tài liệu này gom những công thức cốt lõi để xử lý phần lớn bài Toán 12. Mục tiêu không phải là học thuộc tất cả một lúc, mà là biết:

- Bài dạng nào thì dùng công cụ nào.
- Công thức nào là công thức "áp vào là ra".
- Cần kiểm tra điều kiện gì để tránh sai.

> Cách học nhanh: đọc mỗi mục theo thứ tự **nhận dạng bài -> công thức -> quy trình làm**. Khi làm bài, quay lại đúng mục liên quan, không cần nhớ hết ngay từ đầu.

## Mục lục

- [1. Đạo hàm và nguyên hàm](#1-đạo-hàm-và-nguyên-hàm)
- [2. Khảo sát hàm số](#2-khảo-sát-hàm-số)
- [3. Tiệm cận](#3-tiệm-cận)
- [4. Tích phân và ứng dụng](#4-tích-phân-và-ứng-dụng)
- [5. Vectơ trong không gian](#5-vectơ-trong-không-gian)
- [6. Tọa độ Oxyz](#6-tọa-độ-oxyz)
- [7. Mặt phẳng, đường thẳng, mặt cầu](#7-mặt-phẳng-đường-thẳng-mặt-cầu)
- [8. Mũ, logarit và số phức](#8-mũ-logarit-và-số-phức)
- [9. Xác suất](#9-xác-suất)
- [10. Checklist làm bài](#10-checklist-làm-bài)

## 1. Đạo hàm và nguyên hàm

Đạo hàm dùng để tìm tăng giảm, cực trị, min-max, tiếp tuyến, khảo sát đồ thị. Nguyên hàm và tích phân dùng để tính diện tích, thể tích, giá trị trung bình.

### 1.1 Quy tắc đạo hàm

Với $u = u(x)$, $v = v(x)$ là các hàm khả vi:

| Dạng | Đạo hàm |
|---|---:|
| $(u + v)'$ | $u' + v'$ |
| $(u - v)'$ | $u' - v'$ |
| $(ku)'$ | $ku'$ |
| $(uv)'$ | $u'v + uv'$ |
| $\left(\dfrac{u}{v}\right)'$ | $\dfrac{u'v - uv'}{v^2}$ |
| $(f(u))'$ | $f'(u)u'$ |

### 1.2 Bảng đạo hàm cần nhớ

| Hàm số | Đạo hàm |
|---|---:|
| $x^n$ | $nx^{n-1}$ |
| $\dfrac{1}{x}$ | $-\dfrac{1}{x^2}$ |
| $\sqrt{x}$ | $\dfrac{1}{2\sqrt{x}}$ |
| $e^x$ | $e^x$ |
| $a^x$ | $a^x\ln a$ |
| $\ln x$ | $\dfrac{1}{x}$ |
| $\log_a x$ | $\dfrac{1}{x\ln a}$ |
| $\sin x$ | $\cos x$ |
| $\cos x$ | $-\sin x$ |
| $\tan x$ | $\dfrac{1}{\cos^2 x}$ |
| $\cot x$ | $-\dfrac{1}{\sin^2 x}$ |

Với hàm hợp, thay $x$ bằng $u$ và nhân thêm $u'$:

| Hàm hợp | Đạo hàm |
|---|---:|
| $u^n$ | $nu^{n-1}u'$ |
| $e^u$ | $u'e^u$ |
| $a^u$ | $u'a^u\ln a$ |
| $\ln u$ | $\dfrac{u'}{u}$ |
| $\sin u$ | $u'\cos u$ |
| $\cos u$ | $-u'\sin u$ |
| $\tan u$ | $\dfrac{u'}{\cos^2 u}$ |

### 1.3 Bảng nguyên hàm cần nhớ

| Hàm số | Nguyên hàm |
|---|---:|
| $x^\alpha$, $\alpha \ne -1$ | $\displaystyle\int x^\alpha\,dx = \dfrac{x^{\alpha+1}}{\alpha+1} + C$ |
| $\dfrac{1}{x}$ | $\displaystyle\int \dfrac{1}{x}\,dx = \ln\lvert x\rvert + C$ |
| $e^x$ | $\displaystyle\int e^x\,dx = e^x + C$ |
| $a^x$ | $\displaystyle\int a^x\,dx = \dfrac{a^x}{\ln a} + C$ |
| $\sin x$ | $\displaystyle\int \sin x\,dx = -\cos x + C$ |
| $\cos x$ | $\displaystyle\int \cos x\,dx = \sin x + C$ |
| $\dfrac{1}{\cos^2 x}$ | $\displaystyle\int \dfrac{1}{\cos^2 x}\,dx = \tan x + C$ |
| $\dfrac{1}{\sin^2 x}$ | $\displaystyle\int \dfrac{1}{\sin^2 x}\,dx = -\cot x + C$ |

Nếu gặp hàm hợp tuyến tính $ax+b$, thường chia thêm cho hệ số $a$:

| Dạng | Nguyên hàm |
|---|---:|
| $(ax+b)^\alpha$, $\alpha \ne -1$ | $\dfrac{(ax+b)^{\alpha+1}}{a(\alpha+1)} + C$ |
| $\dfrac{1}{ax+b}$ | $\dfrac{1}{a}\ln\lvert ax+b\rvert + C$ |
| $e^{ax+b}$ | $\dfrac{1}{a}e^{ax+b} + C$ |
| $\sin(ax+b)$ | $-\dfrac{1}{a}\cos(ax+b) + C$ |
| $\cos(ax+b)$ | $\dfrac{1}{a}\sin(ax+b) + C$ |

## 2. Khảo sát hàm số

Đây là dạng bài trung tâm của Toán 12. Gần như mọi câu đều xoay quanh $y'$, dấu của $y'$ và giá trị của $y$ tại các điểm đặc biệt.

### 2.1 Quy trình chuẩn

1. Tìm tập xác định $D$.
2. Tính $y'$.
3. Giải $y' = 0$ và tìm các điểm $y'$ không xác định nếu có.
4. Lập bảng biến thiên: chia trục số theo các điểm vừa tìm, xét dấu $y'$.
5. Kết luận đồng biến, nghịch biến, cực trị, min-max, tiệm cận, đồ thị.

### 2.2 Đơn điệu

| Điều kiện | Kết luận |
|---|---|
| $y' > 0$ trên khoảng | Hàm số đồng biến trên khoảng đó |
| $y' < 0$ trên khoảng | Hàm số nghịch biến trên khoảng đó |
| $y'$ đổi dấu từ $+$ sang $-$ tại $x_0$ | $x_0$ là điểm cực đại |
| $y'$ đổi dấu từ $-$ sang $+$ tại $x_0$ | $x_0$ là điểm cực tiểu |

### 2.3 Min-max

Với bài tìm giá trị lớn nhất, nhỏ nhất trên đoạn $[a;b]$:

1. Tính $y'$.
2. Giải $y'=0$ trong $(a;b)$.
3. Tính $f(a)$, $f(b)$ và $f(x_i)$ với các nghiệm $x_i$.
4. So sánh các giá trị vừa tính.

Kết luận:

- Số lớn nhất là $\max f(x)$.
- Số nhỏ nhất là $\min f(x)$.

### 2.4 Tiếp tuyến

Phương trình tiếp tuyến của đồ thị $y=f(x)$ tại $x=x_0$:

$$
y = f'(x_0)(x-x_0) + f(x_0).
$$

Nếu đề bài cho hoành độ tiếp điểm, thay trực tiếp vào. Nếu đề bài cho hệ số góc $k$, giải $f'(x)=k$ để tìm tiếp điểm.

## 3. Tiệm cận

Tiệm cận giúp nhìn hình dạng đồ thị khi $x$ tiến ra vô cực hoặc tiến đến điểm làm hàm không xác định.

| Loại tiệm cận | Cách tìm |
|---|---|
| Tiệm cận đứng $x=x_0$ | Nếu $\lim\limits_{x\to x_0^+}f(x)=\pm\infty$ hoặc $\lim\limits_{x\to x_0^-}f(x)=\pm\infty$ |
| Tiệm cận ngang $y=y_0$ | Nếu $\lim\limits_{x\to\pm\infty}f(x)=y_0$ |
| Tiệm cận xiên $y=ax+b$ | Nếu $\lim\limits_{x\to\pm\infty}[f(x)-(ax+b)]=0$ |

Với tiệm cận xiên:

$$
\begin{aligned}
a &= \lim_{x\to\pm\infty}\frac{f(x)}{x},\\
b &= \lim_{x\to\pm\infty}\left[f(x)-ax\right].
\end{aligned}
$$

## 4. Tích phân và ứng dụng

### 4.1 Định nghĩa tích phân

Nếu $f(x)$ liên tục trên $[a;b]$ và $F(x)$ là một nguyên hàm của $f(x)$ trên $[a;b]$, thì:

$$
\int_a^b f(x)\,dx = F(b)-F(a).
$$

Nếu $G(x)$ cũng là một nguyên hàm của $f(x)$ thì $G(x)=F(x)+C$, nên $G(b)-G(a)=F(b)-F(a)$.

### 4.2 Tính chất tích phân

| Tính chất | Công thức |
|---|---:|
| Đưa hằng số ra ngoài | $\displaystyle\int_a^b kf(x)\,dx = k\int_a^b f(x)\,dx$ |
| Cộng hai hàm | $\displaystyle\int_a^b [f(x)+g(x)]\,dx = \int_a^b f(x)\,dx+\int_a^b g(x)\,dx$ |
| Trừ hai hàm | $\displaystyle\int_a^b [f(x)-g(x)]\,dx = \int_a^b f(x)\,dx-\int_a^b g(x)\,dx$ |
| Tách cận | $\displaystyle\int_a^b f(x)\,dx = \int_a^c f(x)\,dx+\int_c^b f(x)\,dx$ với $a<c<b$ |

Thêm hai tính chất hay dùng:

$$
\int_a^a f(x)\,dx=0,\qquad
\int_a^b f(x)\,dx=-\int_b^a f(x)\,dx.
$$

### 4.3 Diện tích hình phẳng

Diện tích hình phẳng giới hạn bởi $y=f(x)$, trục hoành và hai đường $x=a$, $x=b$:

$$
S=\int_a^b |f(x)|\,dx.
$$

Nếu miền phẳng nằm giữa hai đồ thị $y=f(x)$ và $y=g(x)$:

$$
S=\int_a^b |f(x)-g(x)|\,dx.
$$

Mẹo làm bài: tìm giao điểm bằng cách giải $f(x)=g(x)$, chia khoảng theo giao điểm, rồi bỏ dấu giá trị tuyệt đối theo "hàm nằm trên trừ hàm nằm dưới".

### 4.4 Giá trị trung bình của hàm số

Giá trị trung bình của hàm liên tục $f(x)$ trên $[a;b]$:

$$
f_{\text{tb}}=\frac{1}{b-a}\int_a^b f(x)\,dx.
$$

### 4.5 Thể tích vật thể theo mặt cắt

Nếu vật thể bị cắt vuông góc với trục $Ox$ tại hoành độ $x$ và diện tích mặt cắt là $S(x)$, với $S(x)$ liên tục trên $[a;b]$, thì thể tích:

$$
V=\int_a^b S(x)\,dx.
$$

### 4.6 Thể tích khối tròn xoay

Cho $f(x)$ liên tục, không âm trên $[a;b]$. Khi quay hình phẳng giới hạn bởi $y=f(x)$, trục hoành, $x=a$, $x=b$ quanh trục $Ox$, thể tích khối tròn xoay là:

$$
V=\pi\int_a^b f^2(x)\,dx.
$$

## 5. Vectơ trong không gian

### 5.1 Tọa độ và phép toán vectơ

Với $A(x_A,y_A,z_A)$, $B(x_B,y_B,z_B)$:

$$
\vec{AB}=(x_B-x_A,\ y_B-y_A,\ z_B-z_A).
$$

Nếu $\vec{a}=(x,y,z)$, $\vec{b}=(x',y',z')$:

| Phép toán | Công thức |
|---|---:|
| Cộng | $\vec{a}+\vec{b}=(x+x',y+y',z+z')$ |
| Trừ | $\vec{a}-\vec{b}=(x-x',y-y',z-z')$ |
| Nhân với số $k$ | $k\vec{a}=(kx,ky,kz)$ |
| Độ dài | $\|\vec{a}\|=\sqrt{x^2+y^2+z^2}$ |

### 5.2 Tích vô hướng và góc giữa hai vectơ

$$
\vec{a}\cdot\vec{b}=xx'+yy'+zz'.
$$

Hai vectơ vuông góc khi và chỉ khi:

$$
\vec{a}\cdot\vec{b}=0.
$$

Nếu $\vec{a}$ và $\vec{b}$ khác $\vec{0}$:

$$
\cos(\vec{a},\vec{b})
=\frac{\vec{a}\cdot\vec{b}}{\|\vec{a}\|\|\vec{b}\|}
=\frac{xx'+yy'+zz'}{\sqrt{x^2+y^2+z^2}\sqrt{x'^2+y'^2+z'^2}}.
$$

### 5.3 Tích có hướng

Cho $\vec{u}=(a,b,c)$ và $\vec{v}=(a',b',c')$. Một vectơ vuông góc với cả $\vec{u}$ và $\vec{v}$ là:

$$
[\vec{u},\vec{v}]
=(bc'-b'c,\ ca'-c'a,\ ab'-a'b).
$$

Dạng định thức, viết ổn định hơn bằng `det`:

$$
[\vec{u},\vec{v}]
=\left(
\det\begin{pmatrix}b&c\\ b'&c'\end{pmatrix},
\det\begin{pmatrix}c&a\\ c'&a'\end{pmatrix},
\det\begin{pmatrix}a&b\\ a'&b'\end{pmatrix}
\right).
$$

Ghi nhớ:

- $[\vec{u},\vec{v}]$ vuông góc với cả $\vec{u}$ và $\vec{v}$.
- $[\vec{u},\vec{v}]=\vec{0}$ khi và chỉ khi $\vec{u}$, $\vec{v}$ cùng phương.
- Khi mặt phẳng có hai vectơ nằm trên nó, lấy tích có hướng của hai vectơ đó sẽ được một vectơ pháp tuyến.

## 6. Tọa độ Oxyz

### 6.1 Điểm, trung điểm, trọng tâm

Với $A(x_A,y_A,z_A)$, $B(x_B,y_B,z_B)$:

$$
I\left(\frac{x_A+x_B}{2},\frac{y_A+y_B}{2},\frac{z_A+z_B}{2}\right)
$$

là trung điểm của $AB$.

Với tam giác $ABC$, trọng tâm:

$$
G\left(
\frac{x_A+x_B+x_C}{3},
\frac{y_A+y_B+y_C}{3},
\frac{z_A+z_B+z_C}{3}
\right).
$$

### 6.2 Khoảng cách hai điểm

$$
AB=\sqrt{(x_B-x_A)^2+(y_B-y_A)^2+(z_B-z_A)^2}.
$$

### 6.3 Kiểm tra thẳng hàng, đồng phẳng

Ba điểm $A,B,C$ thẳng hàng khi $\vec{AB}$ và $\vec{AC}$ cùng phương:

$$
\vec{AB}=k\vec{AC}.
$$

Bốn điểm $A,B,C,D$ đồng phẳng khi:

$$
[\vec{AB},\vec{AC}]\cdot\vec{AD}=0.
$$

## 7. Mặt phẳng, đường thẳng, mặt cầu

### 7.1 Vectơ pháp tuyến và phương trình mặt phẳng

Mặt phẳng $(P): Ax+By+Cz+D=0$ có vectơ pháp tuyến:

$$
\vec{n}=(A,B,C).
$$

Nếu mặt phẳng đi qua $M_0(x_0,y_0,z_0)$ và có vectơ pháp tuyến $\vec{n}=(A,B,C)$:

$$
A(x-x_0)+B(y-y_0)+C(z-z_0)=0.
$$

Nếu mặt phẳng có hai vectơ nằm trên nó là $\vec{u}$, $\vec{v}$, chọn:

$$
\vec{n}=[\vec{u},\vec{v}].
$$

### 7.2 Hai mặt phẳng vuông góc

Cho:

$$
(\alpha): Ax+By+Cz+D=0,\qquad
(\beta): A'x+B'y+C'z+D'=0.
$$

Vectơ pháp tuyến tương ứng:

$$
\vec{n}=(A,B,C),\qquad \vec{n'}=(A',B',C').
$$

Hai mặt phẳng vuông góc khi:

$$
\begin{aligned}
(\alpha)\perp(\beta)
&\Longleftrightarrow \vec{n}\perp\vec{n'}\\
&\Longleftrightarrow AA'+BB'+CC'=0.
\end{aligned}
$$

### 7.3 Hai mặt phẳng song song

Với hai mặt phẳng ở trên:

$$
(\alpha)\parallel(\beta)
\Longleftrightarrow
\begin{cases}
\vec{n'}=k\vec{n},\\
D'\ne kD
\end{cases}
$$

với một số $k$ nào đó. Nếu $\vec{n'}=k\vec{n}$ và $D'=kD$ thì hai mặt phẳng trùng nhau.

### 7.4 Khoảng cách từ điểm đến mặt phẳng

Khoảng cách từ $M(x_0,y_0,z_0)$ đến mặt phẳng $(P): Ax+By+Cz+D=0$:

$$
d(M,(P))=\frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}.
$$

### 7.5 Vectơ chỉ phương và đường thẳng

Vectơ chỉ phương của đường thẳng là vectơ song song hoặc nằm trên đường thẳng.

Nếu đường thẳng $d$ đi qua $M_0(x_0,y_0,z_0)$ và có vectơ chỉ phương $\vec{u}=(a,b,c)$, phương trình tham số:

$$
\begin{cases}
x=x_0+at,\\
y=y_0+bt,\\
z=z_0+ct.
\end{cases}
$$

Nếu $abc\ne0$, phương trình chính tắc:

$$
\frac{x-x_0}{a}=\frac{y-y_0}{b}=\frac{z-z_0}{c}.
$$

### 7.6 Góc giữa hai đường thẳng

Nếu hai đường thẳng có vectơ chỉ phương $\vec{u}_1=(a_1,b_1,c_1)$ và $\vec{u}_2=(a_2,b_2,c_2)$:

$$
\begin{aligned}
\cos\varphi
&= \frac{\left|\vec{u}_1\cdot\vec{u}_2\right|}{\|\vec{u}_1\|\|\vec{u}_2\|}\\
&= \frac{|a_1a_2+b_1b_2+c_1c_2|}
{\sqrt{a_1^2+b_1^2+c_1^2}\sqrt{a_2^2+b_2^2+c_2^2}}.
\end{aligned}
$$

Hai đường thẳng vuông góc khi:

$$
\vec{u}_1\cdot\vec{u}_2=0.
$$

### 7.7 Góc giữa đường thẳng và mặt phẳng

Nếu đường thẳng $d$ có vectơ chỉ phương $\vec{u}$, mặt phẳng $(P)$ có vectơ pháp tuyến $\vec{n}$, góc giữa $d$ và $(P)$ là $\alpha$:

$$
\sin\alpha=\frac{\left|\vec{u}\cdot\vec{n}\right|}{\|\vec{u}\|\|\vec{n}\|}.
$$

### 7.8 Góc giữa hai mặt phẳng

Góc giữa hai mặt phẳng bằng góc giữa hai vectơ pháp tuyến của chúng:

$$
\cos\varphi=
\frac{\left|\vec{n}_1\cdot\vec{n}_2\right|}
{\|\vec{n}_1\|\|\vec{n}_2\|}.
$$

### 7.9 Mặt cầu

Mặt cầu tâm $I(a,b,c)$, bán kính $R$:

$$
(x-a)^2+(y-b)^2+(z-c)^2=R^2.
$$

Dạng tổng quát:

$$
x^2+y^2+z^2+Ax+By+Cz+D=0.
$$

Tâm và bán kính:

$$
I\left(-\frac{A}{2},-\frac{B}{2},-\frac{C}{2}\right),\qquad
R=\sqrt{\frac{A^2+B^2+C^2}{4}-D}.
$$

Điều kiện là:

$$
\frac{A^2+B^2+C^2}{4}-D>0.
$$

## 8. Mũ, logarit và số phức

### 8.1 Mũ và logarit

Điều kiện cần nhớ:

- $a^x$ xác định với $a>0$.
- $\log_a f(x)$ xác định khi $a>0$, $a\ne1$, $f(x)>0$.
- $\ln f(x)$ xác định khi $f(x)>0$.

Công thức logarit:

| Công thức | Điều kiện |
|---|---|
| $\log_a(xy)=\log_a x+\log_a y$ | $x>0,y>0$ |
| $\log_a\left(\dfrac{x}{y}\right)=\log_a x-\log_a y$ | $x>0,y>0$ |
| $\log_a x^\alpha=\alpha\log_a x$ | $x>0$ |
| $\log_a b=\dfrac{\ln b}{\ln a}$ | $a,b>0,a\ne1$ |

### 8.2 Số phức

Số phức có dạng:

$$
z=a+bi,\qquad i^2=-1.
$$

| Khái niệm | Công thức |
|---|---:|
| Phần thực | $a$ |
| Phần ảo | $b$ |
| Số phức liên hợp | $\overline{z}=a-bi$ |
| Mô đun | $|z|=\sqrt{a^2+b^2}$ |
| Tích với liên hợp | $z\overline{z}=|z|^2=a^2+b^2$ |

Nói cách khác, nếu $z=a+bi$ thì phần thực là $a$, phần ảo là $b$.

Chia số phức:

$$
\frac{z_1}{z_2}=\frac{z_1\overline{z_2}}{z_2\overline{z_2}},\qquad z_2\ne0.
$$

## 9. Xác suất

Phần xác suất thường không khó vì công thức dài, mà khó ở chỗ nhận ra biến cố nào là "điều kiện đã biết" và biến cố nào là "kết quả cần tính".

### 9.1 Ký hiệu cơ bản

| Ký hiệu | Ý nghĩa |
|---|---|
| $A$, $B$ | Biến cố |
| $\overline{A}$ | Biến cố đối của $A$ |
| $A\cap B$ | $A$ và $B$ cùng xảy ra |
| $A\cup B$ | $A$ hoặc $B$ xảy ra |
| $P(A)$ | Xác suất của biến cố $A$ |
| $P(A\mid B)$ | Xác suất của $A$ khi biết $B$ đã xảy ra |

Hai công thức nền:

$$
P(\overline{A})=1-P(A).
$$

$$
P(A\cup B)=P(A)+P(B)-P(A\cap B).
$$

Nếu $A$ và $B$ xung khắc, tức là không thể cùng xảy ra, thì:

$$
P(A\cap B)=0,\qquad P(A\cup B)=P(A)+P(B).
$$

### 9.2 Xác suất có điều kiện

Xác suất của $A$ khi biết $B$ đã xảy ra:

$$
P(A\mid B)=\frac{P(A\cap B)}{P(B)},\qquad P(B)>0.
$$

Từ đó suy ra công thức nhân:

$$
P(A\cap B)=P(B)P(A\mid B)=P(A)P(B\mid A).
$$

Cách đọc nhanh:

- $P(A\mid B)$: đang đứng trong thế giới mà $B$ đã xảy ra, hỏi khả năng $A$ xảy ra.
- $P(B\mid A)$: đang đứng trong thế giới mà $A$ đã xảy ra, hỏi khả năng $B$ xảy ra.

Hai xác suất này thường khác nhau, nên không được tự đổi chỗ $A$ và $B$.

### 9.3 Biến cố độc lập

$A$ và $B$ độc lập nếu việc $B$ xảy ra không làm thay đổi xác suất của $A$:

$$
P(A\mid B)=P(A).
$$

Tương đương:

$$
P(A\cap B)=P(A)P(B).
$$

Mẹo nhận dạng: nếu đề nói "chọn/lấy/thực hiện độc lập", "lặp lại trong cùng điều kiện", hoặc kết quả lần này không ảnh hưởng lần kia, thường nghĩ đến công thức độc lập.

### 9.4 Công thức xác suất toàn phần

Giả sử $B_1,B_2,\ldots,B_n$ là một hệ biến cố đầy đủ, nghĩa là:

- Các $B_i$ đôi một xung khắc.
- Chắc chắn có đúng một trong các $B_i$ xảy ra.
- $P(B_i)>0$ với mọi $i$.

Khi đó:

$$
P(A)=P(B_1)P(A\mid B_1)+P(B_2)P(A\mid B_2)+\cdots+P(B_n)P(A\mid B_n).
$$

Viết gọn:

$$
P(A)=\sum_{i=1}^{n}P(B_i)P(A\mid B_i).
$$

Trường hợp hay gặp nhất là tách theo $B$ và $\overline{B}$:

$$
P(A)=P(B)P(A\mid B)+P(\overline{B})P(A\mid \overline{B}).
$$

Cách hiểu: muốn tính xác suất $A$, ta chia bài toán thành nhiều "con đường" dẫn đến $A$, rồi cộng xác suất của từng con đường.

### 9.5 Công thức Bayes

Bayes dùng khi đề cho xác suất "đi xuôi" $P(A\mid B_i)$, nhưng hỏi xác suất "truy ngược" $P(B_i\mid A)$.

Với hệ biến cố đầy đủ $B_1,B_2,\ldots,B_n$:

$$
P(B_k\mid A)
=\frac{P(B_k)P(A\mid B_k)}
{\sum_{i=1}^{n}P(B_i)P(A\mid B_i)}.
$$

Trường hợp chỉ có $B$ và $\overline{B}$:

$$
P(B\mid A)
=\frac{P(B)P(A\mid B)}
{P(B)P(A\mid B)+P(\overline{B})P(A\mid \overline{B})}.
$$

### 9.6 Quy trình làm bài xác suất có điều kiện

1. Gọi rõ biến cố cần tìm, ví dụ $A$: "người được chọn bị bệnh", $B$: "test dương tính".
2. Xác định đề đang hỏi $P(A)$, $P(A\mid B)$ hay $P(B\mid A)$.
3. Nếu bài có nhiều nhóm/trường hợp, đặt các nhóm là $B_1,B_2,\ldots,B_n$.
4. Tính mẫu số bằng xác suất toàn phần nếu cần.
5. Nếu hỏi "biết kết quả rồi truy ngược nguyên nhân", dùng Bayes.

Ví dụ nhận dạng nhanh:

- "Biết rằng test dương tính, xác suất người đó thật sự mắc bệnh là bao nhiêu?" -> Bayes.
- "Một sản phẩm lấy từ nhà máy bất kỳ, xác suất bị lỗi là bao nhiêu?" -> Xác suất toàn phần.
- "Biết đã chọn học sinh lớp 12A, xác suất học sinh đó giỏi Toán là bao nhiêu?" -> Xác suất có điều kiện.

## 10. Checklist làm bài

### 10.1 Gặp bài hàm số

1. Tìm tập xác định.
2. Tính $y'$.
3. Giải $y'=0$.
4. Xét dấu $y'$.
5. Kết luận theo câu hỏi: đồng biến, cực trị, min-max, đồ thị, tiệm cận.

### 10.2 Gặp bài tích phân

1. Nhận dạng dạng cơ bản hay cần đổi biến/từng phần.
2. Nếu là tích phân xác định, tìm nguyên hàm $F(x)$.
3. Tính $F(b)-F(a)$.
4. Nếu là diện tích, nhớ lấy giá trị tuyệt đối hoặc chia khoảng.
5. Nếu là thể tích tròn xoay, nhớ bình phương bán kính và nhân $\pi$.

### 10.3 Gặp bài Oxyz

1. Đổi tất cả về vectơ.
2. Cần vuông góc thì dùng tích vô hướng $=0$.
3. Cần vectơ pháp tuyến thì dùng tích có hướng.
4. Cần mặt phẳng thì cần một điểm và một vectơ pháp tuyến.
5. Cần đường thẳng thì cần một điểm và một vectơ chỉ phương.
6. Cần khoảng cách điểm đến mặt phẳng thì thay vào công thức.

### 10.4 Gặp bài xác suất

1. Đặt tên biến cố rõ ràng.
2. Xác định đề hỏi xác suất thường, xác suất có điều kiện, toàn phần hay Bayes.
3. Nếu có nhiều trường hợp, chia thành hệ biến cố đầy đủ.
4. Tính từng nhánh bằng công thức nhân.
5. Cộng các nhánh nếu dùng xác suất toàn phần, hoặc lấy tỉ lệ nếu dùng Bayes.


// Bonus
Dưới đây là tóm tắt súc tích nhất để bạn nắm trọn quy trình:
## 1. Cách chọn điểm $A$ từ giao tuyến 2 mặt phẳng
Đường thẳng $\Delta$ là giao của $(P)$ và $(Q)$. Để tìm $A \in \Delta$:

* Cách làm: Chọn đại một ẩn ($x, y$ hoặc $z$) bằng một số cụ thể (thường chọn bằng $0$), sau đó giải hệ 2 phương trình còn lại.
* Ví dụ: Cho $z = 0$, giải hệ $\begin{cases} (P) \\ (Q) \end{cases} \Rightarrow$ tìm được $x, y$. Ta có $A(x; y; 0)$.

## 2. Cách suy ra công thức (Dựa vào diện tích)
Công thức: $d(M, \Delta) = \frac{|[\vec{AM}, \vec{u}]|}{|\vec{u}|}$
Suy luận nhanh:

   1. Diện tích hình bình hành: Độ lớn tích có hướng $|[\vec{AM}, \vec{u}]|$ chính là diện tích hình bình hành tạo bởi vectơ nối điểm ($\vec{AM}$) và vectơ chỉ phương ($\vec{u}$).
   2. Chiều cao hình bình hành: Mặt khác, Diện tích = Đáy $\times$ Cao $\Rightarrow S = |\vec{u}| \cdot h$.
   3. Kết quả: Khoảng cách $h$ chính là chiều cao. Vậy $h = \frac{S}{\text{Đáy}} = \frac{|[\vec{AM}, \vec{u}]|}{|\vec{u}|}$.

## 3. Lưu ý để hoàn thiện bài toán
Để tính được, bạn cần thêm vectơ chỉ phương $\vec{u}$:

* $\vec{u} = [\vec{n_P}, \vec{n_Q}]$ (Tích có hướng của hai vectơ pháp tuyến của hai mặt phẳng).

Bạn có cần tôi tính thử một bài tập cụ thể với số liệu thực tế để kiểm tra lại công thức không?

Trong không gian $Oxyz$, cho hai vectơ $\vec{a} = (a_1, a_2, a_3)$ và $\vec{b} = (b_1, b_2, b_3)$. Tích có hướng của chúng là một vectơ, ký hiệu là $[\vec{a}, \vec{b}]$ hoặc $\vec{a} \times \vec{b}$, được tính theo công thức:
$$[\vec{a}, \vec{b}] = \left( \begin{vmatrix} a_2 & a_3 \\ b_2 & b_3 \end{vmatrix}; \begin{vmatrix} a_3 & a_1 \\ b_3 & b_1 \end{vmatrix}; \begin{vmatrix} a_1 & a_2 \\ b_1 & b_2 \end{vmatrix} \right)$$ 
Cách tính từng thành phần (định thức $2 \times 2$):
Công thức nhân chéo: $\begin{vmatrix} e & f \\ g & h \end{vmatrix} = e \cdot h - f \cdot g$

   1. Tọa độ $x$: Che cột thứ nhất, tính định thức 2 cột còn lại.
   2. Tọa độ $y$: Che cột thứ hai, tính định thức cột 3 và cột 1 (theo đúng thứ tự xoay vòng).
   3. Tọa độ $z$: Che cột thứ ba, tính định thức 2 cột đầu.

Mẹo nhớ nhanh:
Viết tọa độ hai vectơ thành hai hàng, viết thêm cột thứ nhất và thứ hai vào phía sau:
$a_1 \quad a_2 \quad a_3 \quad a_1 \quad a_2$
$b_1 \quad b_2 \quad b_3 \quad b_1 \quad b_2$
Bắt đầu từ cột 2, nhân chéo từng cặp 2x2 kế tiếp nhau sẽ ra lần lượt tọa độ $x, y, z$.
Ứng dụng trong bài toán của bạn:
Để tìm vectơ chỉ phương $\vec{u}$ của giao tuyến hai mặt phẳng, bạn chỉ cần lấy tích có hướng của hai vectơ pháp tuyến: $\vec{u} = [\vec{n_1}, \vec{n_2}]$.


