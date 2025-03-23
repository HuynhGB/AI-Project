# Langchain & RAG for LLM
## Giới thiệu
  - Chương trình được xây dựng bằng Langchain, kết hợp với mô hình ngôn ngữ lớn (LLM) nhằm đưa ra nhiều đề xuất về công việc cần phải làm trong ngày hôm nay hoặc những việc đã hoàn thành trong ngày để nhân viên trong công ty có thể lựa chọn.
  - Ở đây chúng ta sử dụng cả model Llama3 trên VPS của công ty và OpenAI để so sánh hiệu suất của cả hai mô hình.
## Quy trình 
  - Mô hình sẽ lấy dữ liệu bao gồm những lần ghi chú trước kia của một nhân viên bất kì và đưa vào file pdf để có thể dự đoán được ngày hôm đó cần phải làm gì hoặc ngày hôm đó đã làm được những công việc gì, đồng thời xuất ra những ghi chú tuỳ chọn.
  - Trường hợp nếu không có lịch sử trước đó thì mô hình sẽ tự dự đoán dựa trên những gì mô hình được train.
  - Sau khi dự đoán xong chương trình sẽ tự động xoá file pdf để mô hình có thể dự đoán mà không bị nhằm lẫn với lịch sử ghi chú của các nhân viên khác.
## Format của dữ liệu
  - Tên dự án, tên task và mô tả của task đó (Trong đó tên dự án là quan trọng nhất và không được thiếu)
## Tính năng
  - Đưa ra suggested next steps khi mới vào công ty check in trên Odoo.
  - Đưa ra suggested work notes khi đã hoàn thành xong công việc của ngày hôm đó trên Odoo.

