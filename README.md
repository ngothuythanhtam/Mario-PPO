# Train AI how to play Super Mario Bros using PPO algorithm
![image](https://github.com/user-attachments/assets/dca0577d-9852-4a1a-8537-10e1c7b60868)

![image](https://github.com/user-attachments/assets/972302db-e923-40ae-817d-39b8e6afdde3)
Đánh giá mô hình huấn luyện
Trong phần này, mô hình huấn luyện sẽ được phân tích hiệu suất qua các bước thời gian đào tạo khác nhau. Ta đánh giá lối chơi của tác nhân và phân tích về những cải tiến quan sát được khi quá trình đào tạo tiến triển. 
 
Đánh giá ở 10K bước: 
•	Hiệu suất: Tác nhân thể hiện sự tiến bộ ban đầu trong việc hiểu cơ chế trò chơi nhưng thiếu thành thạo trong việc điều hướng để vượt các chướng ngại vật. 
•	Quan sát: Tác nhân gặp khó khăn khi di chuyển qua các ống thường xuyên không vượt qua được chướng ngại vật. 
•	Phân tích: Ở giai đoạn đào tạo ban đầu này, tác nhân đang trong giai đoạn học tập ban đầu và cần phải đào tạo bổ sung để nâng cao hiệu suất của nó. 

Đánh giá ở 100K bước: 
•	Hiệu suất: Lối chơi của đặc vụ kém đi, thể hiện kỹ năng điều hướng kém. 
•	Quan sát: Đặc vụ liên tục không vượt qua được ống thứ 2, dẫn đến mất mạng thường xuyên. 
•	Phân tích: Mặc dù được đào tạo bổ sung, tác nhân vẫn tiếp tục gặp khó khăn trong việc tìm hiểu chiến lược điều hướng tối ưu. 

Đánh giá ở 1M bước: 
•	Hiệu suất: Tác nhân thể hiện sự tiến bộ đáng kể và thể hiện sự thành thạo trong việc giải quyết các chướng ngại vật. 
•	Quan sát: Tác nhân thành công vượt qua chướng ngại vật và hoàn thành cấp độ thế giới 1-1 nhưng cần mất nhiều thời gian. 
•	Phân tích: Thời gian đào tạo kéo dài đã cho phép tác nhân phát triển sự hiểu biết tốt hơn về cơ chế trò chơi và cải thiện kỹ năng điều hướng của mình.

Đánh giá ở 2M bước:
•	Hiệu suất: Tác nhân thành thạo vượt qua các chướng ngại vật với số phần thưởng cao. 
•	Quan sát: Tác nhân thành công hoàn thành cấp độ thế giới 1-1 nhưng vẫn mất rất nhiều thời gian. 
•	Phân tích: Thời gian đào tạo kéo dài đã cho phép tác nhân phát triển sự hiểu biết tốt hơn về cơ chế trò chơi và mang lại số điểm cao hơn.

Đánh giá ở 3M bước:
•	Hiệu suất: Tác nhân tiếp tục thể hiện hiện sự thành thạo trong việc giải quyết các chướng ngại vật. 
•	Quan sát: Tác nhân đụng độ Goomba một lần nhưng hồi sinh và thành công vượt qua chướng ngại vật để hoàn thành cấp độ thế giới 1-1. 
•	Phân tích: Thời gian đào tạo kéo dài đã cho phép tác nhân phát triển sự hiểu biết tốt hơn về cơ chế trò chơi và cải thiện kỹ năng điều hướng của mình.

Đánh giá ở 4M bước: 
•	Hiệu suất: Tác nhân thể hiện hiệu suất kém. 
•	Quan sát: Tác nhân thể hiện các chuyển động chính xác và tiếp cận thành công ống thứ ba nhưng gặp khó khăn khi tiến xa hơn. 
•	Phân tích: Cần phải điều chỉnh thêm, chẳng hạn như sử dụng tốc độ học thấp hơn để thông ống thứ ba. Mô hình hiện tại đã được huấn luyện với tốc độ học tập là 0,000001 và không thể vượt qua thế giới 1-1 ở mức 4M bước, cho thấy mức độ học tập chưa phù hợp.

Đánh giá ở 5M bước:
•	Hiệu suất: Tác nhân thể hiện sự tiến bộ hơn so với hiệu suất ở 4M bước. 
•	Quan sát: Tác nhân thành công vượt qua ống thứ 3 và tiến về đích nhưng cần mất rất nhiều thời gian. 
•	Phân tích: Với quá trình đào tạo kéo dài, tác nhân đã đạt được tiến bộ khi vượt qua các ống và các Goomba . 

Đánh giá ở 6M bước:
•	Hiệu suất: Tác nhân thể hiện hiệu suất kém. 
•	Quan sát: Tác nhân liên tục bị rơi xuống hố thứ 3. 
•	Phân tích: Với quá trình đào tạo chuyên sâu, tác nhân đã đạt được tiến bộ khi vượt qua các ống và các Goomba . Tuy nhiên, cần phải điều chỉnh thêm, chẳng hạn như sử dụng tốc độ học thấp hơn để vượt qua hố thứ 3. 

Đánh giá ở 7M bước: 
•	Hiệu suất: Tác nhân vẫn thể hiện hiệu suất kém. 
•	Quan sát: Tác nhân liên tục không tránh được Goomba khi nhảy qua ống thứ 2. 
•	Phân tích: Kịch bản này nêu bật những nhược điểm của việc sử dụng tốc độ học cao. Tác nhân liên tục không vượt qua chướng ngại vật . 
 
Đánh giá ở 8M bước:
•	Hiệu suất: Tác nhân tiến bộ hơn so với mức 7M bước. 
•	Quan sát: Tác nhân gặp chút khó khăn để để vượt qua bức tường gạch nhưng vẫn thành công hoàn thành cấp độ thế giới 1-1. 
•	Phân tích: Mặc dù thời gian đào tạo kéo dài nhưng tác nhân chưa rút ngắn được thời gian hoàn thành cấp độ.

Đánh giá ở 9M bước: 
•	Hiệu suất: Tác nhân tiếp tục thể hiện sự tiến bộ. 
•	Quan sát: Tác nhân thành công vượt qua các chướng ngại vật và hoàn thành cấp độ thế giới 1-1. 
•	Phân tích: Mặc dù thời gian đào tạo kéo dài nhưng tác nhân vẫn cần mất nhiều thời gian để hoàn thành.

Đánh giá ở 10M bước:
•	Hiệu suất: Tác nhân tiếp tục thể hiện hiệu suất tiến bộ.
•	Quan sát: Tác nhân gặp khó khăn khi vượt qua hố thứ 3, nhưng sau nhiều lần thử tác nhân cũng đã vượt qua và hoàn thành cấp độ thế giới 1-1. 
•	Phân tích: Dù đã huấn luyện đến 10 triệu bước nhưng phần thưởng tác nhân đạt được vẫn còn thấp, chưa tối đa hóa được phần thưởng và thời gian hoàn thành khá lâu. Cần phải điều chỉnh thêm, chẳng hạn như sử dụng tốc độ học thấp hơn để vượt qua các chướng ngại vật và điều chỉnh lại số n_steps để tác nhân học tập kỹ hơn. 

(Tải file .doc để xem thêm chi tiết)
