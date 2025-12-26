# Lời giải đề CTRR (CO1007) - HK 231

---

**Câu 1.** Có hai lô sản phẩm A và B. Lô A có 10 sản phẩm loại I, và 2 sản phẩm loại II. Lô B có 16 sản phẩm loại I và 4 sản phẩm loại II. Từ mỗi lô, lấy ngẫu nhiên ra một sản phẩm. Sau đó, từ 2 sản phẩm thu được lấy ngẫu nhiên ra một sản phẩm cuối cùng. Xác suất sản phẩm cuối là loại I là bao nhiêu?

A. 0.59  
B. 0.69  
C. 0.79  
D. 0.89

**Lời giải:**
Ta có thể giải bài này bằng cách chia thành các trường hợp

- Trường hợp 1: lô `A` - loại `I`, lô `B` - loại `II`:
Khi đó xác suất để lấy được sản phẩm loại `I` sẽ là
$$P_1 =\dfrac{10}{12}\times\dfrac{4}{20} \times \dfrac{1}{2} = \dfrac{1}{12}$$

- Trường hợp 2: lô `A` - loại `II`, lô `B` - loại `I`
Khi đó xác suất để lấy được sản phẩm loại `I` sẽ là
$$P_2 = \dfrac{2}{12} \times \dfrac{16}{20} \times \dfrac{1}{2} = \dfrac{1}{15}$$
- Trường hợp 3: cả 2 lô đều bốc được loại `I`
Khi đó xác suất để lấy được sản phẩm loại `I` sẽ là
$$P_3 = \dfrac{10}{12}\times \dfrac{16}{20}\times 1 = \dfrac{2}{3}$$

**Vậy xác suất để lấy ra được một sản phẩm loại 1 là**
$$P = \sum P_i = P_1 + P_2 + P_3 = \dfrac{1}{12} + \dfrac{1}{15} + \dfrac{2}{3} \approx 0.8167$$

Như vậy không có đáp án nào trong đề thoả mãn.

---

**Câu 2.** Giả sử bộ lọc thư rác Bayesian được huấn luyện trên một bộ dữ liệu gồm 500 thư rác và 200 thư không phải thư rác. Từ "exciting" xuất hiện trong 40 thư rác và 25 tin nhắn không phải thư rác. Tính xác suất một thư đến bị coi là thư rác nếu nó chứa từ "exciting"? (Giả sử, để đơn giản, thư có khả năng là thư rác và không phải là thư rác là như nhau.)

A. 0.59  
B. 0.61  
C. 0.39  
D. 0.41

**Lời giải:**
Gọi các biến cố lần lượt là:

- $A$: thư rác.
- $\overline{A}$: không phải thư rác.
- $B$: có chứa từ exciting.
- $\overline{B}$: Không chứa từ exciting.

Từ đề bài ta có:

- $P(B|A) = \frac{40}{500}$
- $P(B|\overline{A}) = \frac{25}{200}$

Ta cần tính giá trị $P(A|B)$. Theo định lý `Bayes` ta có:
\[P(A|B) = \dfrac{P(B|A) \times P(A)}{P(B|A) \times P(A)+P(B|\overline{A}) \times P(\overline{A})} = \dfrac{\frac{40}{500}\times\frac{1}{2}}{\frac{40}{500}\times\frac{1}{2}+\frac{25}{200}\times\frac{1}{2}} \approx 0.39\]
