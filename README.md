> [!CAUTION]
> * This entire README is written in Vietnamese, as my English is quite poor
> * However, I may add other languages ​​in the future if possible

> [!NOTE]
> * Tool này có sự đóng góp (chắc là khá nhiều) từ AI, nhưng không phải toàn bộ là AI mà tui cũng có đóng góp nhé
> * Tui là một coder chỉ mới học Py gần 2 tháng, nếu có lỗi gì mong ae chỉ bảo 🐧
***
<p align="center">
<pre align="center">
  __  _______    ____  __   ___   
  \ \/ /_  _/   / __ \/ /  / _ \  
   \  / / /  = / /_/ / /__/ ___/  
   /_/ /_/     \____/____/_/      
      D O W N L O A D E R      
</pre>
</p>

## Table Of Content
   1. [Giới thiệu](#-yt-dlp-với-giao-diện-tui)
   2. [Screenshot](#-screenshot)
   3. [Tính năng](#-tính-năng)
   4. [Cách tải / sử dụng](#-cách-tải--sử-dụng)
      - [Cách tải](#-cách-tải)
      - [Cách sử dụng](#-cách-dùng)
   5. [Vấn đề đã biết](#-vấn-đề-đã-biết)


# 😋 YT-DLP với giao diện TUI
<p align="center">
  <img width="80%" alt="Main menu" src="https://github.com/user-attachments/assets/14b7e1d6-24dc-4b99-8c8b-8e315aecc979" />
</p>
  
Vài một ngày đẹp trời nào đó, tôi đang tìm trang web phù hợp với mình để tải video youtube thì phát hiện [yt-dlp][1]. Quá ngon, tôi liền tải về và thử nó một thời gian thì nhận ra: `yt-dlp` không chỉ có download video mà còn có thể lựa chọn format, chỉnh resolution, cắt video trực tiếp, ... Nhưng với bộ não cá vàng của tôi thì việc nhớ đến đống câu lệnh vô cảm là không thể.

Sau đó, tôi dành khá nhiều thời gian để tìm các công cụ dùng `yt-dlp` có chứa các tính năng trên để sử dụng, tuy nhiên đa số đều không có, hoặc nếu có thì hoạt động quá chậm, kém hiệu quả và có lúc chả hoạt động.

Và một ý tưởng hiện ra trong đầu tôi: thay vì tìm kiếm trên mạng thì sao mình không tự làm đi nhỉ. Sau đó tôi liền bắt tay vào làm cùng con Gemini của Google. Tham khảo code, giao diện và idea từ nhiều nguồn, tôi đã tạo ra `YT-DLP downloader` :DD

# 📷 Screenshot
  

<p align="center">
  <img width="80%" alt="nhap-link" src="https://github.com/user-attachments/assets/8e127a34-56d4-4d58-882d-77bf85eff25d" /><br>
  <i>Nhập link</i><br><br>
  <img width="80%" alt="chon-quality" src="https://github.com/user-attachments/assets/113ba014-366f-4830-a785-978226c34b6e" /><br>
  <i>Chọn chất lượng media</i><br><br>
  <img width="80%"" alt="trim-media" src="https://github.com/user-attachments/assets/0312b5c9-419e-4c23-8723-1ea484b571ba" /><br>
  <i>Cắt media</i><br><br>
  <img width="80%" alt="result" src="https://github.com/user-attachments/assets/89d8033a-14f0-4d5c-a22d-b012cc13d84f" /><br>
  <i>Hoàn thiện</i><br><br>
</p>

# 🚀 Tính năng

Như đã nói ở trên thì `YT-DLP downloader` sẽ chứa các tính năng mà tôi muốn và có thể tiếp cận bằng `yt-dlp`

### Tính năng cơ bản
- Tải media từ 1000+ các trang khác nhau
> (nó nói thế chứ tôi kbt nữa, tôi chỉ dùng để tải video youtube với facebook thôi 🐧)
- Giao diện thân thiện với ~~tôi~~ người dùng
- Cho phép chuyển đổi qua lại giữa mp3 / mp4
- Cho phép tuỳ chỉnh chất lượng video
- Các file tải về sẽ được bỏ vào thư mục `download`

### Tính năng nâng cao
- Có thể cắt media bằng cách nhập thời gian bắt đầu / kết thúc
- Cho phép tải được nhiều file chỉ trong một lần nhấp

# 📦 Cách tải / sử dụng
## 📥 Cách tải
Bên dưới sẽ là những gì cần có và cách tải cụ thể
### ⚠ Yêu cầu thiết yếu
Đây là những thứ cần phải có để chương trình hoạt động:
- [ ] [Python](https://www.python.org/) (v3.10+ đối với CPython / 3.11+ đối với PyPy)
- [x] [YT-DLP][1]
- [x] `ffmpeg` và `ffprobe`
> `YT-DLP`, `ffmpeg` và `ffprobe` đã có sẵn nên chỉ cần tải thêm Python thôi

### 🏌️‍♀️ Installation
- Step 1️⃣: Tải `ytdl-vX.X.rar` mới nhất ở **Release** hoặc bấm vào [đây](https://github.com/NDKcute/YT-DLP_downloader/releases)
- Step 2️⃣: Giải nén file `ytdl-vX.X.rar` trên vào ổ đĩa `C:`
- Step 3️⃣: Mở thư mục vừa giải nén, chạy file `yt-dlp downloader.bat` và dùng thôi 🥳


## 🕹 Cách dùng
```text
                              __  ______     ____  __   ___
                              \ \/ /_  _/   / __ \/ /  / _ \
                               \  / / /  = / /_/ / /__/ ___/
                               /_/ /_/     \____/____/_/
                                   D O W N L O A D E R

            ╭────────────┐┌─ [2] Nhập link ──────────────────┐┌─────────────╮
            │ [1] mp4 v  ││ > ...                            ││ [3] 720p v  │
            ╰────────────┘└──────────────────────────────────┘└─────────────╯

                                    >>> (4) START <<<

                  ╭───────────────────── TUỲ CHỌN ─────────────────────╮
                  │                                                    │
                  │  [5] Cắt media              [6] Tải từ links.txt   │
                  │  [7] Mở thư mục tải về      [8] Cập nhật yt-dlp    │
                  │  [9] Exit                                          │
                  │                                                    │
                  ╰────────────────────────────────────────────────────╯

                                  Chọn chức năng (1-9):
```
Ở trên là **giao diện màn hình chính** của `YT-DLP downloader`

- **\[1]**: Chuyển đổi qua lại format **mp3** và **mp4**
- **\[2]**: Nơi để **dán link** cần tải, cho phép **tối đa 5 link** trong một lần tải. Nhấn `` ` `` để thoát thêm link | `x` để **xoá link** bằng cách nhập số thứ tự
- **\[3]**: Thay đổi **chất lượng** của file mp4 (144p, 240p, 360p, 720p, 1080p, Best)
> Đối với mp3: Tự động lấy chất lượng âm thanh tốt nhất
- **\(4)**: **Bắt đầu** quá trình tải xuống
- **\[5]**: **Cắt độ dài media** bằng cách nhập thời gian bắt đầu và thời gian kết thúc. Enter (không nhập gì) để cắt **từ đầu / tới cuối** | Định dạng **HH:MM:SS** hay **MM:SS** đều được
- **\[6]**: **Tải không giới hạn link** trong một lần tải từ file `links.txt` trong đường dẫn `C:\ytdl`, mỗi link tương ứng với **một dòng**. **File được tải về sẽ nhận format và chất lượng ở \[1] và \[3]**
- **\[7]**: Mở thư mục `download` chứa các file media được tải về
- **\[8]**: **Kiểm tra phiên bản mới** của `yt-dlp`. Nên cho chạy định kì để luôn giữ cho `yt-dlp` mới nhất
- **\[9]**: Thoát `YT-DLP downloader`

Chỉ vậy thôi, giờ hãy test tool này với [video youtube](https://youtu.be/dQw4w9WgXcQ?si=geznY5C04ORgMH1J
) này nào!!!

# 🐞 Vấn đề đã biết

_blank_

***
Do là lần đầu viết README.md nên có thể sẽ có sai sót. Cảm ơn mọi người đã đọc :>>



[1]: https://github.com/yt-dlp/yt-dlp
