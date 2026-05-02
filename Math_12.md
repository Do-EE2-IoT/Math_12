# Toan 12 Core - Cong thuc va cach dung nhanh

Tai lieu nay gom nhung cong thuc cot loi de xu ly phan lon bai Toan 12. Muc tieu khong phai la hoc thuoc tat ca mot luc, ma la biet:

- Bai dang nao thi dung cong cu nao.
- Cong thuc nao la "xong viec" nhanh nhat.
- Can kiem tra dieu kien gi de tranh sai.

> Cach hoc nhanh: doc moi muc theo thu tu **Nhan dang bai -> Cong thuc -> Quy trinh lam**. Khi lam bai, quay lai dung muc lien quan, khong can nho het ngay tu dau.

## Muc luc

- [1. Dao ham va nguyen ham](#1-dao-ham-va-nguyen-ham)
- [2. Khao sat ham so](#2-khao-sat-ham-so)
- [3. Tiem can](#3-tiem-can)
- [4. Tich phan va ung dung](#4-tich-phan-va-ung-dung)
- [5. Vecto trong khong gian](#5-vecto-trong-khong-gian)
- [6. Toa do Oxyz](#6-toa-do-oxyz)
- [7. Mat phang, duong thang, mat cau](#7-mat-phang-duong-thang-mat-cau)
- [8. Mu, logarit va so phuc](#8-mu-logarit-va-so-phuc)
- [9. Checklist lam bai](#9-checklist-lam-bai)

## 1. Dao ham va nguyen ham

Dao ham dung de tim tang giam, cuc tri, min-max, tiep tuyen, khao sat do thi. Nguyen ham va tich phan dung de tinh dien tich, the tich, gia tri trung binh.

### 1.1 Quy tac dao ham

Voi $u = u(x)$, $v = v(x)$ la cac ham kha vi:

| Dang | Dao ham |
|---|---:|
| $(u + v)'$ | $u' + v'$ |
| $(u - v)'$ | $u' - v'$ |
| $(ku)'$ | $ku'$ |
| $(uv)'$ | $u'v + uv'$ |
| $\left(\dfrac{u}{v}\right)'$ | $\dfrac{u'v - uv'}{v^2}$ |
| $(f(u))'$ | $f'(u)u'$ |

### 1.2 Bang dao ham can nho

| Ham so | Dao ham |
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

Voi ham hop, thay $x$ bang $u$ va nhan them $u'$:

| Ham hop | Dao ham |
|---|---:|
| $u^n$ | $nu^{n-1}u'$ |
| $e^u$ | $u'e^u$ |
| $a^u$ | $u'a^u\ln a$ |
| $\ln u$ | $\dfrac{u'}{u}$ |
| $\sin u$ | $u'\cos u$ |
| $\cos u$ | $-u'\sin u$ |
| $\tan u$ | $\dfrac{u'}{\cos^2 u}$ |

### 1.3 Bang nguyen ham can nho

| Ham so | Nguyen ham |
|---|---:|
| $x^\alpha$, $\alpha \ne -1$ | $\displaystyle\int x^\alpha\,dx = \dfrac{x^{\alpha+1}}{\alpha+1} + C$ |
| $\dfrac{1}{x}$ | $\displaystyle\int \dfrac{1}{x}\,dx = \ln\lvert x\rvert + C$ |
| $e^x$ | $\displaystyle\int e^x\,dx = e^x + C$ |
| $a^x$ | $\displaystyle\int a^x\,dx = \dfrac{a^x}{\ln a} + C$ |
| $\sin x$ | $\displaystyle\int \sin x\,dx = -\cos x + C$ |
| $\cos x$ | $\displaystyle\int \cos x\,dx = \sin x + C$ |
| $\dfrac{1}{\cos^2 x}$ | $\displaystyle\int \dfrac{1}{\cos^2 x}\,dx = \tan x + C$ |
| $\dfrac{1}{\sin^2 x}$ | $\displaystyle\int \dfrac{1}{\sin^2 x}\,dx = -\cot x + C$ |

Neu gap ham hop tuyen tinh $ax+b$, thuong chia them cho he so $a$:

| Dang | Nguyen ham |
|---|---:|
| $(ax+b)^\alpha$, $\alpha \ne -1$ | $\dfrac{(ax+b)^{\alpha+1}}{a(\alpha+1)} + C$ |
| $\dfrac{1}{ax+b}$ | $\dfrac{1}{a}\ln\lvert ax+b\rvert + C$ |
| $e^{ax+b}$ | $\dfrac{1}{a}e^{ax+b} + C$ |
| $\sin(ax+b)$ | $-\dfrac{1}{a}\cos(ax+b) + C$ |
| $\cos(ax+b)$ | $\dfrac{1}{a}\sin(ax+b) + C$ |

## 2. Khao sat ham so

Day la dang bai trung tam cua Toan 12. Gan nhu moi cau deu xoay quanh $y'$, dau cua $y'$ va gia tri cua $y$ tai cac diem dac biet.

### 2.1 Quy trinh chuan

1. Tim tap xac dinh $D$.
2. Tinh $y'$.
3. Giai $y' = 0$ va tim cac diem $y'$ khong xac dinh neu co.
4. Lap bang bien thien: chia truc so theo cac diem vua tim, xet dau $y'$.
5. Ket luan dong bien, nghich bien, cuc tri, min-max, tiem can, do thi.

### 2.2 Don dieu

| Dieu kien | Ket luan |
|---|---|
| $y' > 0$ tren khoang | Ham so dong bien tren khoang do |
| $y' < 0$ tren khoang | Ham so nghich bien tren khoang do |
| $y'$ doi dau tu $+$ sang $-$ tai $x_0$ | $x_0$ la diem cuc dai |
| $y'$ doi dau tu $-$ sang $+$ tai $x_0$ | $x_0$ la diem cuc tieu |

### 2.3 Min-max

Voi bai tim gia tri lon nhat, nho nhat tren doan $[a;b]$:

1. Tinh $y'$.
2. Giai $y'=0$ trong $(a;b)$.
3. Tinh $f(a)$, $f(b)$ va $f(x_i)$ voi cac nghiem $x_i$.
4. So sanh cac gia tri vua tinh.

Ket luan:

- So lon nhat la $\max f(x)$.
- So nho nhat la $\min f(x)$.

### 2.4 Tiep tuyen

Phuong trinh tiep tuyen cua do thi $y=f(x)$ tai $x=x_0$:

$$
y = f'(x_0)(x-x_0) + f(x_0).
$$

Neu de bai cho hoanh do tiep diem, thay truc tiep vao. Neu de bai cho he so goc $k$, giai $f'(x)=k$ de tim tiep diem.

## 3. Tiem can

Tiem can giup nhin hinh dang do thi khi $x$ tien ra vo cuc hoac tien den diem lam ham "no tung".

| Loai tiem can | Cach tim |
|---|---|
| Tiem can dung $x=x_0$ | Neu $\lim\limits_{x\to x_0^+}f(x)=\pm\infty$ hoac $\lim\limits_{x\to x_0^-}f(x)=\pm\infty$ |
| Tiem can ngang $y=y_0$ | Neu $\lim\limits_{x\to\pm\infty}f(x)=y_0$ |
| Tiem can xien $y=ax+b$ | Neu $\lim\limits_{x\to\pm\infty}[f(x)-(ax+b)]=0$ |

Voi tiem can xien:

$$
a=\lim_{x\to\pm\infty}\frac{f(x)}{x},\qquad
b=\lim_{x\to\pm\infty}\left[f(x)-ax\right].
$$

## 4. Tich phan va ung dung

### 4.1 Dinh nghia tich phan

Neu $f(x)$ lien tuc tren $[a;b]$ va $F(x)$ la mot nguyen ham cua $f(x)$ tren $[a;b]$, thi:

$$
\int_a^b f(x)\,dx = F(b)-F(a).
$$

Neu $G(x)$ cung la mot nguyen ham cua $f(x)$ thi $G(x)=F(x)+C$, nen $G(b)-G(a)=F(b)-F(a)$.

### 4.2 Tinh chat tich phan

| Tinh chat | Cong thuc |
|---|---:|
| Dua hang so ra ngoai | $\displaystyle\int_a^b kf(x)\,dx = k\int_a^b f(x)\,dx$ |
| Cong hai ham | $\displaystyle\int_a^b [f(x)+g(x)]\,dx = \int_a^b f(x)\,dx+\int_a^b g(x)\,dx$ |
| Tru hai ham | $\displaystyle\int_a^b [f(x)-g(x)]\,dx = \int_a^b f(x)\,dx-\int_a^b g(x)\,dx$ |
| Tach can | $\displaystyle\int_a^b f(x)\,dx = \int_a^c f(x)\,dx+\int_c^b f(x)\,dx$ voi $a<c<b$ |

Them hai tinh chat hay dung:

$$
\int_a^a f(x)\,dx=0,\qquad
\int_a^b f(x)\,dx=-\int_b^a f(x)\,dx.
$$

### 4.3 Dien tich hinh phang

Dien tich hinh phang gioi han boi $y=f(x)$, truc hoanh va hai duong $x=a$, $x=b$:

$$
S=\int_a^b |f(x)|\,dx.
$$

Neu mien phang nam giua hai do thi $y=f(x)$ va $y=g(x)$:

$$
S=\int_a^b |f(x)-g(x)|\,dx.
$$

Meo lam bai: tim giao diem bang cach giai $f(x)=g(x)$, chia khoang theo giao diem, roi bo dau gia tri tuyet doi theo ham nam tren tru ham nam duoi.

### 4.4 Gia tri trung binh cua ham so

Gia tri trung binh cua ham lien tuc $f(x)$ tren $[a;b]$:

$$
f_{\text{tb}}=\frac{1}{b-a}\int_a^b f(x)\,dx.
$$

### 4.5 The tich vat the theo mat cat

Neu vat the bi cat vuong goc voi truc $Ox$ tai hoanh do $x$ va dien tich mat cat la $S(x)$, voi $S(x)$ lien tuc tren $[a;b]$, thi the tich:

$$
V=\int_a^b S(x)\,dx.
$$

### 4.6 The tich khoi tron xoay

Cho $f(x)$ lien tuc, khong am tren $[a;b]$. Khi quay hinh phang gioi han boi $y=f(x)$, truc hoanh, $x=a$, $x=b$ quanh truc $Ox$, the tich khoi tron xoay la:

$$
V=\pi\int_a^b f^2(x)\,dx.
$$

Neu quay mien giua hai ham $f(x)$ va $g(x)$ quanh truc $Ox$, thuong dung:

$$
V=\pi\int_a^b \left(R^2(x)-r^2(x)\right)\,dx,
$$

trong do $R(x)$ la ban kinh lon, $r(x)$ la ban kinh nho.

## 5. Vecto trong khong gian

### 5.1 Toa do va phep toan vecto

Voi $A(x_A,y_A,z_A)$, $B(x_B,y_B,z_B)$:

$$
\vec{AB}=(x_B-x_A,\ y_B-y_A,\ z_B-z_A).
$$

Neu $\vec{a}=(x,y,z)$, $\vec{b}=(x',y',z')$:

| Phep toan | Cong thuc |
|---|---:|
| Cong | $\vec{a}+\vec{b}=(x+x',y+y',z+z')$ |
| Tru | $\vec{a}-\vec{b}=(x-x',y-y',z-z')$ |
| Nhan voi so $k$ | $k\vec{a}=(kx,ky,kz)$ |
| Do dai | $\lvert\vec{a}\rvert=\sqrt{x^2+y^2+z^2}$ |

### 5.2 Tich vo huong va goc giua hai vecto

$$
\vec{a}\cdot\vec{b}=xx'+yy'+zz'.
$$

Hai vecto vuong goc khi va chi khi:

$$
\vec{a}\cdot\vec{b}=0.
$$

Neu $\vec{a}$ va $\vec{b}$ khac $\vec{0}$:

$$
\cos(\vec{a},\vec{b})
=\frac{\vec{a}\cdot\vec{b}}{\lvert\vec{a}\rvert\lvert\vec{b}\rvert}
=\frac{xx'+yy'+zz'}{\sqrt{x^2+y^2+z^2}\sqrt{x'^2+y'^2+z'^2}}.
$$

### 5.3 Tich co huong

Cho $\vec{u}=(a,b,c)$ va $\vec{v}=(a',b',c')$. Mot vecto vuong goc voi ca $\vec{u}$ va $\vec{v}$ la:

$$
[\vec{u},\vec{v}]
=(bc'-b'c,\ ca'-c'a,\ ab'-a'b).
$$

Dang dinh thuc:

$$
[\vec{u},\vec{v}]
=\left(
\begin{vmatrix}b&c\\b'&c'\end{vmatrix},
\begin{vmatrix}c&a\\c'&a'\end{vmatrix},
\begin{vmatrix}a&b\\a'&b'\end{vmatrix}
\right).
$$

Ghi nho:

- $[\vec{u},\vec{v}]$ vuong goc voi ca $\vec{u}$ va $\vec{v}$.
- $[\vec{u},\vec{v}]=\vec{0}$ khi va chi khi $\vec{u}$, $\vec{v}$ cung phuong.
- Khi mat phang co hai vecto nam tren no, lay tich co huong cua hai vecto do se duoc mot vecto phap tuyen.

## 6. Toa do Oxyz

### 6.1 Diem, trung diem, trong tam

Voi $A(x_A,y_A,z_A)$, $B(x_B,y_B,z_B)$:

$$
I\left(\frac{x_A+x_B}{2},\frac{y_A+y_B}{2},\frac{z_A+z_B}{2}\right)
$$

la trung diem cua $AB$.

Voi tam giac $ABC$, trong tam:

$$
G\left(
\frac{x_A+x_B+x_C}{3},
\frac{y_A+y_B+y_C}{3},
\frac{z_A+z_B+z_C}{3}
\right).
$$

### 6.2 Khoang cach hai diem

$$
AB=\sqrt{(x_B-x_A)^2+(y_B-y_A)^2+(z_B-z_A)^2}.
$$

### 6.3 Kiem tra thang hang, dong phang

Ba diem $A,B,C$ thang hang khi $\vec{AB}$ va $\vec{AC}$ cung phuong:

$$
\vec{AB}=k\vec{AC}.
$$

Bon diem $A,B,C,D$ dong phang khi:

$$
[\vec{AB},\vec{AC}]\cdot\vec{AD}=0.
$$

## 7. Mat phang, duong thang, mat cau

### 7.1 Vecto phap tuyen va phuong trinh mat phang

Mat phang $(P): Ax+By+Cz+D=0$ co vecto phap tuyen:

$$
\vec{n}=(A,B,C).
$$

Neu mat phang di qua $M_0(x_0,y_0,z_0)$ va co vecto phap tuyen $\vec{n}=(A,B,C)$:

$$
A(x-x_0)+B(y-y_0)+C(z-z_0)=0.
$$

Neu mat phang co hai vecto nam tren no la $\vec{u}$, $\vec{v}$, chon:

$$
\vec{n}=[\vec{u},\vec{v}].
$$

### 7.2 Hai mat phang vuong goc

Cho:

$$
(\alpha): Ax+By+Cz+D=0,\qquad
(\beta): A'x+B'y+C'z+D'=0.
$$

Vecto phap tuyen tuong ung:

$$
\vec{n}=(A,B,C),\qquad \vec{n'}=(A',B',C').
$$

Hai mat phang vuong goc khi:

$$
(\alpha)\perp(\beta)
\Longleftrightarrow
\vec{n}\perp\vec{n'}
\Longleftrightarrow
AA'+BB'+CC'=0.
$$

### 7.3 Hai mat phang song song

Voi hai mat phang o tren:

$$
(\alpha)\parallel(\beta)
\Longleftrightarrow
\begin{cases}
\vec{n'}=k\vec{n},\\
D'\ne kD
\end{cases}
$$

voi mot so $k$ nao do. Neu $\vec{n'}=k\vec{n}$ va $D'=kD$ thi hai mat phang trung nhau.

### 7.4 Khoang cach tu diem den mat phang

Khoang cach tu $M(x_0,y_0,z_0)$ den mat phang $(P): Ax+By+Cz+D=0$:

$$
d(M,(P))=\frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}.
$$

### 7.5 Vecto chi phuong va duong thang

Vecto chi phuong cua duong thang la vecto song song hoac nam tren duong thang.

Neu duong thang $d$ di qua $M_0(x_0,y_0,z_0)$ va co vecto chi phuong $\vec{u}=(a,b,c)$, phuong trinh tham so:

$$
\begin{cases}
x=x_0+at,\\
y=y_0+bt,\\
z=z_0+ct.
\end{cases}
$$

Neu $abc\ne0$, phuong trinh chinh tac:

$$
\frac{x-x_0}{a}=\frac{y-y_0}{b}=\frac{z-z_0}{c}.
$$

### 7.6 Goc giua hai duong thang

Neu hai duong thang co vecto chi phuong $\vec{u}_1=(a_1,b_1,c_1)$ va $\vec{u}_2=(a_2,b_2,c_2)$:

$$
\cos\varphi=
\frac{|\vec{u}_1\cdot\vec{u}_2|}
{\lvert\vec{u}_1\rvert\lvert\vec{u}_2\rvert}
=
\frac{|a_1a_2+b_1b_2+c_1c_2|}
{\sqrt{a_1^2+b_1^2+c_1^2}\sqrt{a_2^2+b_2^2+c_2^2}}.
$$

Hai duong thang vuong goc khi:

$$
\vec{u}_1\cdot\vec{u}_2=0.
$$

### 7.7 Goc giua duong thang va mat phang

Neu duong thang $d$ co vecto chi phuong $\vec{u}$, mat phang $(P)$ co vecto phap tuyen $\vec{n}$, goc giua $d$ va $(P)$ la $\alpha$:

$$
\sin\alpha=\frac{|\vec{u}\cdot\vec{n}|}{|\vec{u}||\vec{n}|}.
$$

### 7.8 Goc giua hai mat phang

Goc giua hai mat phang bang goc giua hai vecto phap tuyen cua chung:

$$
\cos\varphi=
\frac{|\vec{n}_1\cdot\vec{n}_2|}
{|\vec{n}_1||\vec{n}_2|}.
$$

### 7.9 Mat cau

Mat cau tam $I(a,b,c)$, ban kinh $R$:

$$
(x-a)^2+(y-b)^2+(z-c)^2=R^2.
$$

Dang tong quat:

$$
x^2+y^2+z^2+Ax+By+Cz+D=0.
$$

Tam va ban kinh:

$$
I\left(-\frac{A}{2},-\frac{B}{2},-\frac{C}{2}\right),\qquad
R=\sqrt{\frac{A^2+B^2+C^2}{4}-D}.
$$

Dieu kien la:

$$
\frac{A^2+B^2+C^2}{4}-D>0.
$$

## 8. Mu, logarit va so phuc

### 8.1 Mu va logarit

Dieu kien can nho:

- $a^x$ xac dinh voi $a>0$, $a\ne1$ neu lam logarit co co so $a$.
- $\log_a f(x)$ xac dinh khi $a>0$, $a\ne1$, $f(x)>0$.
- $\ln f(x)$ xac dinh khi $f(x)>0$.

Cong thuc logarit:

| Cong thuc | Dieu kien |
|---|---|
| $\log_a(xy)=\log_a x+\log_a y$ | $x>0,y>0$ |
| $\log_a\left(\dfrac{x}{y}\right)=\log_a x-\log_a y$ | $x>0,y>0$ |
| $\log_a x^\alpha=\alpha\log_a x$ | $x>0$ |
| $\log_a b=\dfrac{\ln b}{\ln a}$ | $a,b>0,a\ne1$ |

### 8.2 So phuc

So phuc co dang:

$$
z=a+bi,\qquad i^2=-1.
$$

| Khai niem | Cong thuc |
|---|---:|
| Phan thuc | $\operatorname{Re}(z)=a$ |
| Phan ao | $\operatorname{Im}(z)=b$ |
| So phuc lien hop | $\overline{z}=a-bi$ |
| Mo dun | $|z|=\sqrt{a^2+b^2}$ |
| Tich voi lien hop | $z\overline{z}=|z|^2=a^2+b^2$ |

Chia so phuc:

$$
\frac{z_1}{z_2}=\frac{z_1\overline{z_2}}{z_2\overline{z_2}},\qquad z_2\ne0.
$$

## 9. Checklist lam bai

### 9.1 Gap bai ham so

1. Tim tap xac dinh.
2. Tinh $y'$.
3. Giai $y'=0$.
4. Xet dau $y'$.
5. Ket luan theo cau hoi: dong bien, cuc tri, min-max, do thi, tiem can.

### 9.2 Gap bai tich phan

1. Nhan dang dang co ban hay can doi bien/tung phan.
2. Neu la tich phan xac dinh, tim nguyen ham $F(x)$.
3. Tinh $F(b)-F(a)$.
4. Neu dien tich, nho lay gia tri tuyet doi hoac chia khoang.
5. Neu the tich tron xoay, nho binh phuong ban kinh va nhan $\pi$.

### 9.3 Gap bai Oxyz

1. Doi tat ca ve vecto.
2. Can vuong goc thi dung tich vo huong $=0$.
3. Can vecto phap tuyen thi dung tich co huong.
4. Can mat phang thi can mot diem va mot vecto phap tuyen.
5. Can duong thang thi can mot diem va mot vecto chi phuong.
6. Can khoang cach diem-den-mat-phang thi thay vao cong thuc.

## Nguon cong thuc tu anh da chuyen thanh Markdown

- [`goc_giua_hai_vecto.png`](./images/goc_giua_hai_vecto.png)
- [`tinh_chat_tich_phan.png`](./images/tinh_chat_tich_phan.png)
- [`tich_phan_mat_s.png`](./images/tich_phan_mat_s.png)
- [`gia_tri_trung_binh_hamso.png`](./images/gia_tri_trung_binh_hamso.png)
- [`tichphan_the_tich.png`](./images/tichphan_the_tich.png)
- [`the_tich_khoi_tron_xoay.png`](./images/the_tich_khoi_tron_xoay.png)
- [`vecto_phap_tuyen.png`](./images/vecto_phap_tuyen.png)
- [`hai_mat_phang_vuong_goc.png`](./images/hai_mat_phang_vuong_goc.png)
- [`hai_mat_phang_song_song.png`](./images/hai_mat_phang_song_song.png)
- [`mot_Diemt_toi_1_mp.png`](./images/mot_Diemt_toi_1_mp.png)
- [`Tinh_goc_giua_hai_duong_thang.png`](./images/Tinh_goc_giua_hai_duong_thang.png)
