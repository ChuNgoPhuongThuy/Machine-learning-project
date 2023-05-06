# Machine-learning-project
Đây là project cuối kỳ môn Học máy (Machine Learning). Project đang trong quá trình hoàn thiện nên không tránh khỏi những sai sót.
### Đề tài: Xử lý bộ dữ liệu chữ số viết tay
#### Dữ liệu:
Bộ dữ liệu chữ số viết tay lấy từ: http://yann.lecun.com/exdb/mnist/

Dữ liệu được để trong 4 tệp với thông tin như dưới đây:

* train-images-idx3-ubyte: training set images (dữ liệu ảnh train)

* train-labels-idx1-ubyte: training set labels (dữ liệu nhãn ứng với ảnh train)

* t10k-images-idx3-ubyte: test set images (dữ liệu ảnh test)

* t10k-labels-idx1-ubyte: test set labels (dữ liệu nhãn ứng với ảnh test)

Tập huấn luyện chứa 60000 mẫu và tập test chứa 10000 mẫu. Chú ý dữ liệu ảnh các chữ số viết tay ở đây được lưu liên tiếp nhau và không theo định dạng ảnh.

Cường độ Pixels được sắp xếp cạnh nhau thành dòng. Giá trị cường độ Pixel là từ 0 đến 255 (1byte) nhưng để ngược: 0 là background (trắng), và 255 là foreground (đen), tuy nhiên khi in ảnh ra màn hình thì điều này không quan trọng.

Ở đây nhãn cho ảnh là số nguyên từ 0 đến 9 (ứng với chữ số trong ảnh). Cấu trúc của tệp dữ liệu ảnh test (train-images-idx3-ubyte) và nhãn ảnh test (t10k-labels-idx1-ubyte) tương tự như với dữ liệu training, số lượng ảnh là 10000.

#### Yêu cầu đề tài:
##### Yêu cầu 1: 
Thực hiện việc rút gọn số chiều dữ liệu, sau đó tham khảo để hiển thị trực quan các phân lớp dữ liệu dạng 3D hoặc 2D.
* Phương pháp giảm số chiều dữ liệu: Principal Component Analysis (PCA)
* Thư viện xử lý: sklearn
##### Yêu cầu 2: 
Thực hiện phân cụm (clustering) dữ liệu gốc bằng 01 thuật toán phân cụm. Hiển thị trực quan và đánh dấu các cụm.
##### Yêu cầu 3: 
Xây dựng chương trình sử dụng mô hình Multinomial Logistic Regression (Softmax) để phân loại các hình ảnh, huấn luyện mô hình bằng tập dữ liệu training sau đó chạy kiểm tra với dữ liệu trong tập validation.
##### Yêu cầu 4: 
Xây dựng chương trình sử dụng mô hình Multi-Classes Support Vector Machine để phân loại các hình ảnh, huấn luyện mô hình bằng tập dữ liệu training sau đó chạy kiểm tra với dữ liệu trong tập validation.
##### Yêu cầu 5: 
So sánh độ chính xác (sử dụng accuracy, confusion matrix, recall và precision) của các mô hình trong ý 4) và ý 3).
