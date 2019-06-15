# Luận bàn về Máy học (Machine Learning)

**Dùng cho chém gió**
- Lập trình truyền thống: Dữ liệu và chương trình được chạy trên máy tính để tạo đầu ra. 
- Học máy: Dữ liệu và đầu ra được chạy trên máy tính để tạo chương trình. Chương trình này có thể được sử dụng trong lập trình truyền thống.
![](https://3qeqpr26caki16dnhd19sv6by6v-wpengine.netdna-ssl.com/wp-content/uploads/2015/12/Traditional-Programming-vs-Machine-Learning-300x213.png)

**Dùng cho chém gió (P2)**
>Học máy giống như làm nông nghiệp hoặc làm vườn. Hạt giống là thuật toán, chất dinh dưỡng là dữ liệu, người làm vườn là bạn và thực vật là chương trình.

**Explain**
>Từ một bài toán, ta nạp dữ liệu cùng output và dạy cho máy học. Từ đó ta có thể tìm ra một mối liên hệ nhất định trong tập dữ liệu ấy.

**Tiền đề cơ bản by Miss Thương**
Có nhiều phương pháp học khác nhau nhưng tất cả đều phải thoả mãn:
>Dùng một tập quan sát để khám phá một **tiến trình/ quy luật ẩn** bên trong

## Ứng dụng thực tế từ máy học

- Tài chính: quyết định gửi những gì thẻ tín dụng cung cấp cho. Đánh giá rủi ro về cung cấp tín dụng. Cách quyết định đầu tư tiền vào đâu. 
- Thương mại điện tử: Dự đoán khuấy đảo khách hàng. Có hay không một giao dịch là gian lận.
- Khai thác thông tin: Đặt câu hỏi qua cơ sở dữ liệu trên web. 
- Mạng xã hội: Dữ liệu về mối quan hệ và sở thích. Máy học để trích xuất giá trị từ dữ liệu.

## Câu chuyện về thuật toán Máy học
Các thuật toán máy học thường có 3 thành phần:
- Biểu diễn tri thức như neural networks, SVM, cây quyết định,...
- Đánh giá - như việc đánh giá mô hình giả thuyết. Accuracy, Square Error, xác suất, entropy,...
- Tối ưu: nói chung nó sẽ có nhiều hướng để giải quyết bài toán thì ở thuật toán mình có thể điều chỉnh để tối ưu như tối ưu lồi (Gradient Descent) trong Hồi quy tuyến tính (Linear Regression) chẳng hạn.

Tất cả các thuật toán học máy là sự kết hợp của ba thành phần này. Một khuôn khổ để hiểu tất cả các thuật toán.

## Các thể loại học máy - Types of Learning
Nói chung có 4 loại thôi:
- **Học tập có giám sát**: (còn gọi là học tập quy nạp) Dữ liệu đào tạo bao gồm các kết quả mong muốn. Ví dụ như kiểm tra thư rác :)))
- **Học tập không giám sát**: Dữ liệu hỗn loại, đéo biết nó là con cặc gì chỉ biết biểu diễn nó trên toạ độ mà vĩ mô hơn gọi là siêu mặt phẳng. Thì ta sẽ tiến hành gom cụm với các cụm được quy ước sẵn những thuộc tính, tính chất để gom thành 1 nhóm đó. Giống có một đống là và thằng Nhất Minh nó gom thấy mẹ đến nỗi mà lòng nó mơ mơ mơ mơ mơ cc mơ clmm
- **Học bán giám sát**: Dữ liệu đào tạo bao gồm một vài nhóm mong muốn. Như có nhóm chó và nhóm mèo. Mèo chó, chó mèo, chéo mò, chò méo, méo chò, mò chéo. cặc. 
- **Học tăng cường**: Cứ biết  nói là AI bá đạo thống trị thế giới mà điển hình là con Sophia nó có quốc tịch Ả Rập.

## Câu chuyện về xử lý dataset for training

**Offline Learning**
Nói chung đó giờ mình xài Offline Learning thôi là mình xử lý cả khối. Thì giả thuyết đổi full dữ liệu đổi. Mình cũng phân xác suất để tách training set và test set. điển hình thì mình có BGD á . Nếu dữ liệu không real-time thì cách này đánh hiệu suất mô hình rất tốt.
**Online Learning**
Xử lý từng dòng, cứ quẫy lần lượt thì training set, test set nó lẫn cả vào nhau. Và giả thuyết thay đổi dự theo dữ liệu. Nhưng nên nhớ Online là quẫy với real-time nên dữ liệu khó bảo trì và chỉ nên dùng khi:
- Dữ liệu real-time cập nhật liên tục
- Khả năng tính toán & lưu trữ của máy giới hạn

## Câu chuyện về học có giám sát (Supervised Learning)

Học giám sát là bài toán mình được đưa ra các ví dụ về hàm dưới dạng dữ liệu (x) và đầu ra của hàm f(x). 
Mục tiêu của học quy nạp là học hàm cho dữ liệu mới (x), đơn cử:
- Phân lớp (Classification): khi chức năng được học là rời rạc. 
- Hồi quy: khi hàm được học là liên tục.
- Ước tính xác suất: khi đầu ra của hàm là xác suất.

**Tham khảo 2 quan điểm về học giám sát:**
- Học hỏi là loại bỏ sự không chắc chắn. Có dữ liệu loại bỏ một số sự không chắc chắn. Chọn một lớp các giả thuyết, mình sẽ loại bỏ sự không chắc chắn hơn.
- Học là dự đoán một lớp giả thuyết tốt và nhỏ. Mình không biết giải pháp thì phải sử dụng quy trình kiểm thử. 