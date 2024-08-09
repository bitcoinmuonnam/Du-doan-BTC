# Phân tích thị trường Crypto - BTC bằng AI  

***1. Bitcoin***

- Bitcoin (hay biết đến với tên "BTC") vốn là đồng tiền điện tử đầu tiên trên thế giới, do tổ chức Sakoshi Nakamoto phát hành dựa trên phần mềm mã nguồn mở từ năm 2009. Bitcoin có thể được trao đổi trực tiếp bằng thiết bị kết nối Internet mà không cần thông qua một tổ chức tài chính trung gian nào.

![image](https://github.com/user-attachments/assets/24fc6fd0-d3b3-49bb-a1d2-3ea417ef5dc7) ![image](https://github.com/user-attachments/assets/0e2d1b01-a618-4c87-adb7-724c81daa907)
- Bitcoin vốn sinh ra và hoạt động dựa trên giao thức "mạng ngang hàng" (peer-to-peer network), sự cung ứng các tiền ảo đều dựa vào các thuật toán tự động, hạn chế và bao gồm phân chia theo lịch trình giao dịch.  
- Bitcoin được cấp tới các máy tính giao dịch để trả công cho việc xác minh giao dịch Bitcoin và ghi chúng vào "cuốn sổ cái" được phân tán trong hệ thống mạng ngang hàng, thông qua hình thức Blockchain, "cuốn sổ" trên cũng chính là đơn vị kế toán và mỗi bitcoin đều có thể chia nhỏ ra tới 100 triệu đơn vị nhỏ hơn gọi là "satoshi".
- Với giao dịch Bitcoin, phí giao dịch có thể áp dụng mới tuỳ thuộc vào tài nguyên của mạng. Ngoài phí giao dịch, các thợ đào còn được trả công cho việc tạo ra các khối (block) chứa nhật ký giao dịch. Cứ mỗi 10 phút, một khối mới được tạo ra kèm theo một lượng Bitcoin được cấp phát.

***2. Biến động thị trường của BTC***
  - 15 năm sau khởi đầu rất khiêm tốn vào tháng 1/2009, Bitcoin đã làm thay đổi hoàn toàn các thị trường tài chính toàn cầu và đạt được giá trị vốn hóa thị trường hơn 2.000 tỷ USD. Hoạt động giao dịch Bitcoin trực tuyến diễn ra đầu tiên vào năm 2010. Giá đồng tiền này đã tăng từ mức 1 USD/BTC vào năm 2011. Từ đó, giá Bitcoin tiếp tục lên dốc, chạm mức 1.000 USD/BTC vào cuối năm 2013. Bốn năm sau đó, độ phủ sóng và khối lượng giao dịch của đồng tiền này tăng vọt. Vào tháng 11/2017, Bitcoin leo lên mức 10.000 USD/BTC và chạm đỉnh hơn 20.000 USD/BTC chỉ một tháng sau đó.
  - Sau đó, sức nóng của đồng tiền số lớn nhất thế giới đã hạ nhiệt vào năm 2018, khi Bitcoin rơi tự do và để thủng mốc 4.000 USD/BTC. Kéo theo đó, đồng tiền ảo đầu tiên trên thế giới này bắt đầu biến động và giảm dần vào những năm sau đó, bao gồm cả những năm đại dịch COVID-19 và vào năm 2022, Bitcoin mất 60% giá trị còn thị trường tiền mã hóa cũng “bốc hơi” 1,4 nghìn tỷ USD trước áp lực lãi suất tăng.
    
    ![image](https://github.com/user-attachments/assets/64ecc788-77d9-4b92-b4b3-035270868773)
                *Nguồn: TradingView*


***3. AI Bitcoin Prediction***
- Sử dụng datasets từ năm 2014 cho đến năm 2021, kết hợp với thuật toán Decision Tree Regression, *Bitcoin Prediction* sẽ phân tích các biến động của đồng tiền BTC theo từng tháng, trích từng các data giao dịch theo từng timestamps, giá khởi đầu và tỉ giá đồng tiền trên thị trường
- Ma trận dữ liệu nhập vào bao gồm nhiều chiều, bỏ qua các dữ liệu NaN (vốn là dữ liệu mà timestamps không ghi nhận bất cứ giao dịch được thực hiện vào ngày hôm đó), sử dụng thư viện ***Matplotlib, seaborn*** để visulaize biến động lẫn ***sklearn, numpy, pandas*** để thống kê data. Qua đó AI sẽ phân tích các dữ liệu và đưa ra giá trị predict biến động và expected value theo từng ngày thống kê kèm theo actual value. 
