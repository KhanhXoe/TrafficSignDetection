# Bài toán gồm 2 phần chính: 
  + Xây dựng bộ phân loại biển báo:
    - Thuật toán SVM được sử dụng với:
      - Input: Bức ảnh chứa biển báo.
      - Output: Nhãn phân loại của biển báo.
    - Đặc trưng HOG được sử dụng để tạo biểu diễn tốt hơn cho ảnh đầu vào.
  + Xác định vị trí của các biển báo dựa vào bộ phân loại đã xây dựng:
    - Ý tưởng: (Sliding Window)
      - Định nghĩa các cửa sổ trượt trên bức ảnh gốc với kích thước phù hợp.
      - Trượt các cửa sổ này trên các bức ảnh, từ trái qua phải, trên xuống dưới.
      - Mỗi cửa sổ ghi lại được đưa vào bên trong bộ phân loại để xác định liệu cửa sổ có chứa biển báo hay không.
    
