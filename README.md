# Game-ComeBackHome
## :dart: Báo cáo Game ComeBackHome_v1(provide current posistion) and  ComeBackHome_v2( without provide current posistion)

## :dart: Báo cáo Game ComeBackHome bản cho biết vị trí hiện tại
1.   `Tốc độ chạy`
      - **1000000 Game**: 23.2
2. `Chuẩn form`: **Đã test**
3. `Đúng luật`: **Đã check**
4. `Không bị loop vô hạn`: **Đã test** với 1000000 ván
5. `Số ván check_vic > victory_thật`: 10000 ván thì có(thắng thật:2511, check_victory:2511)

## :globe_with_meridians: ENV_state
*   [0:900] **Map của maze**: 1 là tường, 0 là đường có thể đi
*   [900:902] **player position**
*   [902:904] **start position** 
*   [904:906] **end position** 
*   [906] **Turn**
*   [907] **Turn  tối ưu**


## :bust_in_silhouette: P_state
*   [0:2] **vị trí hiện tại** (Bản v1 là vị trí hiện tại còn bản v2 là vị trí điểm bắt đầu)
*   [2:4] **vị trí của đích đến**
*   [4:8] **4 hướng xung quanh có tường hay không**, 4 state gồm: [up,down,left,right]
*   [8]:   **Turn hiện tại**
*   [9]:   **Turn tối ưu**, số turn mà nhanh nhất có thể đi



## :video_game: Action
* [0] **action đi trái**
* [1] **action đi thẳng**
* [2] **action đi lùi**
* [3] **action đi phải**

