# M07_CNN_Transformer_LSTM-GRU
Kiến thức trong M07 bao gồm CNN, Tranformer, LSTM, GRU, ngoài ra còn có Vanishing Gradient

I. LSTM
- Ý tưởng của LSTM là do RNN thường hay bị Vanishing hoặc Exploding Gradient khiến nó không nhớ được lâu. Tách bộ nhớ thành:
  + Short-term memory
  + Long-term memory
 
- Ba thành phần chính của LSTM:
  + Forget Gate: quên đi bao nhiêu thông tin cũ
  + Input Gate: Thêm bao nhiêu thông tin mới
  + Outpuut gate: bao nhiêu thông tin từ memory được đưa ra output

<img width="1266" height="618" alt="{A1778488-0FB1-4AAB-B1EE-BA80DE29C019}" src="https://github.com/user-attachments/assets/06bbd07e-3725-4b17-bf01-34e0420515d3" />
- Hình minh họa 1 LSTM Unit

Câu hỏi: Tại sao trong LSTM lại dùng nhiều loại activation funtion:
- dùng sigmoid cho 3 gate vì nằm trong khoảng (0,1) để biễu diễn % thông tin, hàm tanh (-1, 1) dùng cho memory vì thông tin có thể quan trọng hoặc không quan trọng.

