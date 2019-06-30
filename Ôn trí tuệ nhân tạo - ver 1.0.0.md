# Đề thi  

![](https://i.ytimg.com/vi/kkj9zxPJGis/hqdefault.jpg)

Làm bài 90 ' - đéo sử dụng tài liệu 

## Anh em chém gió

Định nghĩa Trí tuệ nhân tạo đơn thuần chia thành các tư tưởng chính:
1. Cơ sở Tri thức (Knowledge)
- Tầm nhìn (Vision)
2. Khả năng học hỏi (Learning)
3. Suy nghĩ và suy diễn (Think & Deduction)

## /* Luận bàn Kỹ thuật*/

## 1>  Heuristic 

- @What:  Cái mẹ gì là thuật giải Heuristic? 
- @Why: Dùng trong cái gì ?
- @How: Dùng cái mẹ đó ra sao ?
- @When: Cái mẹ đó dùng khi nào ?
- @Pricinples for designing heuristic algorithms: Experience, Vision, 

Heuristic không chính xác cũng được, nhưng độ lệch không cao là oke.

#### Nguyên lý:
- Vét cạn !(ngu xi)
- Tham lam 

### All about A* 

**A-Star ? @Why ? Trong khi địt mẹ xài Djiska cũng được mà ?**

Problem:
- We need to find path, we have algorithms which are omptimized for path finding problems in real life.
- Tìm đường đi ngắn nhất từ đỉnh - đỉnh (Begin: A -> Target:Z).
- Tìm đường đi ngắn nhất từ 1 đỉnh đến các đỉnh còn lại.

#### A little knowedge about Djiska

Input:
- G=(V,E) với w > 0
- Begin vertice: A
- End vertice: Z

Output: The shortest path from A -> Z.

Ký hiệu viết cho mã giả
- Với x thuộc V, g(x) = độ dài lộ trình được tìm thấy từ a -> x.
- Open = tập hợp các đỉnh được duyệt tới nhưng chưa xét các đỉnh kế.
- Close = tập các đỉnh đc duyệt và cũng đã xét các đỉnh kế.
- Pre(x) : đỉnh kế trước x trên lộ trình đến x.

Mã giả:

while open != {} vì
 {
     x thuộc open mà g(x) min; x from open -> close.
     if (x là z) then Dừng & kết luận: find solution
     xét những đỉnh kế y thuộc V - Close của x :
    - TH1: y là đỉnh mới (k thuộc open, close)
         {
            g(y) = g(X) + w(x,y); pre(y) =x; Lưu y trong Open;
         }
    - Th2: y k thuộc open
    {
        g(y) =g(x) + w(x,y)
        Pre(y) =x;
    }
 }

#### A-Star Details
Ký hiệu viết cho mã giả
- Với x thuộc V, g(x) = độ dài lộ trình được tìm thấy từ a -> x.
- Bổ sung h(x) như giả thuyết là f(x) = g(x) + h(x)
- Open = tập hợp các đỉnh được duyệt tới nhưng chưa xét các đỉnh kế.
- Close = tập các đỉnh đc duyệt và cũng đã xét các đỉnh kế.
- Pre(x) : đỉnh kế trước x trên lộ trình đến x.

Lý thuyết:
- Thuật giải dạng mã giả - Dạng mở rộng và cải tiến Djiska.

## 2> Biểu diễn tri thức

### 2.1> Logic vị trừ
- Khái niệm vị từ : Presenting a sentence in Natural Language into a predicate clause.
- **Kỹ thuật: Thuật giải Resolution -> prove a fact** 
- Application

### 2.2> Logic hệ luật dẫn
- Khái niệm hệ luật dẫn
- Model là người mẫu , địt con mẹ nó dẫn cái lozzz

#### Thuật giải Suy diễn tiến - lùi:

**Suy diễn tiến:**

#### Application:
-- pytagore
-- euler trong lý thuyết đồ thị
-- Bài toán tam giác
-- Mô hình hệ luật dẫn: **GT(r) => KL(r)**
### 2.3> Logic mệnh đề
- Kỹ thuật: Thuật giải Robinson, Vương Hạo
### 2.4> Logic mạng ngữ nghĩa (Semantic Network)
### 2.5> Frame, Class in AI


# Expand

Logic mệnh đề bị hạn chế = > Logic mờ (Fuzzy Logic) 
- Chân lý có thể là giá trị là mức độ đúng giữa 0 và 1
- P 0.75 và Q 0.9