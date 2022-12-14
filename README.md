# Game-ComeBackHome
## :dart: Báo cáo Game ComeBackHome bản cho biết vị trí hiện tại
1.   `Tốc độ chạy`
      - **1000000 Game**: 23.2
2. `Chuẩn form`: **Đã test**
3. `Đúng luật`: **Đã check**
4. `Không bị loop vô hạn`: **Đã test** với 1000000 ván
5. `Tốc độ chạy các hàm con mà người chơi dùng`: 1000game: 24s
6. `Số ván check_vic > victory_thật`: 10000 ván thì có(thắng thật:2511, check_victory:2565)
7. `Giá trị state, action:`
9. `Tối thiểu số lần truyền vào player`: 1000 ván, (212, 382) lần truyền vào player

## :globe_with_meridians: ENV_state
*   [0:90] **các thẻ trên bàn**: 5 là đang ở trên bàn, -(p_id) là đang úp, p_id là người chơi đã mua được
*   [100] **Turn**
*   [101:107] **Nguyên liệu trên bàn**, gồm có 6 nguyên liệu
*   [107 + 12 * p_id:119 + 12 * p_id] **thông tin của người chơi**, gồm có  6 nguyên liệu đang có, 5 nguyên liệu mặc định và điểm
*   [155:160] **5 Nguyên liệu mà người đó đã lấy** trong turn
*   [161:164] **3 thẻ ẩn có thể úp** cấp 1, 2, 3

## :bust_in_silhouette: P_state
*   [0:2]  **vị trí của player position **
*   [2: 4] **thông tin của người chơi**, gồm có  6 nguyên liệu đang có, 5 nguyên liệu mặc định và điểm
*   [4:8]: **Các vị trí xung quanh player có tường hay không 
*   [8]:   **Turn
*   [9]:   **Turn Tối ưu 


## :video_game: Action
* [0] **action đi trái**
* [1] **action đi thẳng**
* [2] **action đi lùi**
* [3] **action đi phải**

