<br />
<p align="center">
    <a href="https://github.com/mirairepit/miraiv9">
    </a>

<h3 align="center">MiraiBot</h3>

<p align="center">
    <br />
    <br />
    <a href="https://github.com/mirairepit/miraiv9/issues">Report Bug</a>
    ·
    <a href="https://github.com/mirairepit/miraiv9/pulls">Request Feature</a>
    </p>
</p>

  </p>

<!-- TABLE OF CONTENTS -->
<details open="open">
    <summary>Table of Contents</summary>
    <ol>
        <li><a href="#introduce">Giới thiệu</a></li>
        <li><a href="#Installation">Hướng dẫn cài đặt</a></li>
        <li><a href="#contributing">Contributing</a></li>
        <li><a href="#license">License</a></li>
        <li><a href="#contact">Contact</a></li>
    </ol>
</details>

<!-- ABOUT THE PROJECT -->
## introduce
<p><strong>MIRAIrepit LÀ GÌ?</strong></p>
<br />
<p>
<strong>Mirairepit</strong> thật chất là một dự án mang đến Messenger một trải nghiệm mới cho người dùng bằng cách xây dựng một hệ thống bot dành riêng cho messenger facebook. 
</p>



<!-- INSTALLATION -->
## Installation

Sau đây là các bước cơ bản để có thể cài đặt và vận hành.

### Yêu cầu

- Dung lượng của máy phải trống tầm 1-2gb.
- Cần một số phần mềm chỉnh sửa file, khuyến khích sử dụng [notepad++](https://notepad-plus-plus.org/downloads/) hoặc [sublime text 3](https://www.sublimetext.com/3)
- Cần hiểu biết sơ lược qua về node, javascript.
- Một tài khoản Facebook dùng để làm bot(Khuyến khích nên sử dụng acc đã bỏ hoặc không còn sử dụng để tránh mất acc hay acc bị khoá).
- Đối với:
    - Windows: Cần cài đặt windows-build-tools.
    - Linux: Cần cài đặt python3 hoặc python2.
    - Android Sử dụng termux để vận hành bot.

### Cài Đặt

#### Windows

1. Tải về [Nodejs](https://nodejs.org/en/) và [git](https://git-scm.com/) sau đó cài đặt
    1. Nếu bạn window 7 trở xuống và không thể cài đặt nodejs thì có thể tải file cài đặt nodejs [tại đây(win 64bit)](https://nodejs.org/download/release/v13.14.0/node-v13.14.0-x64.msi) hoặc [tại đây(win 32bit)](https://nodejs.org/download/release/v13.14.0/node-v13.14.0-x86.msi)

2. Cài đặt windows-build-tools:
    1. Mở powershell với quyền adminstrator thông qua startMenu
    2. Nhập 
     ```sh
     npm install windows-build-tools
     ```

3. Clone source code của bot
    1. chuột phải ở folder cần cài đặt source code nhấn vào git bash
    2. nhập
    ```sh
    git clone https://github.com/mirairepit/miraiv9.git miraiv2
    ``` 

4. Cài đặt các package cần thiết
    1. Mở cmd/terminal ở thư mục bot, LƯU Ý thư mục đó phải có file package.json
    2. Nhập
    ```sh
    npm install
    ```

5. Chỉnh sửa file config
    1. Mở file config.json thông qua notepad++ hoặc sublime text 3 đã cài đặt ở trên
    2. tùy chỉnh mail, password, tên bot, ...
    3. Sao lưu và đóng lại

6. Lấy appstate
    - Bạn có thể sử dụng fbstate của c3c bot, nhưng cần đổi tên lại thành appstate.json hoặc đổi lại tên trong phần config.json như bước ở trên
    1. Nhập
    ```sh
    node login
    ```
    2. Nhập mã xác thực hai lớp
    3. Nếu trên cmd/terminal hiện ```Đã ghi xong appstate``` tức là appstate của bạn đã được lưu lại, còn nếu ra dòng có chữ error thì appstate của bạn chưa được lưu lại, bạn cần phải kiểm tra lại thông tin tài khoản, và kiểm tra xem tài khoản của bạn có phải bị checkpoint hay không.

7. Chạy bot và tận hưởng
    1. Nhập
    ```sh
      npm start
      ```
    2. Đợi source code load file và tận hưởng!

#### Android

1. Sử dụng google play và tải termux

2. Mở termux và nhập
    ```sh
    termux-setup-storage && apt update && apt upgrade && pkg install curl -y && bash <(curl -s https://raw.githubusercontent.com/catalizcs/storage-data/master/install.sh)
    ```

3. Đợi mọi package, lib cài đặt thành công là có thể sử dụng

4. Lấy appstate
    - Bạn có thể sử dụng fbstate của c3c bot, nhưng cần đổi tên lại thành appstate.json hoặc đổi lại tên trong config.json
    1. Nhập
    ```sh
    node login
    ```
    2. Nhập mã xác thực hai lớp
    3. Nếu trên cmd/terminal hiện ```Đã ghi xong appstate``` tức là appstate của bạn đã được lưu lại, còn nếu ra dòng có chữ error thì appstate của bạn chưa được lưu lại, bạn cần phải kiểm tra lại thông tin tài khoản, và kiểm tra xem tài khoản của bạn có phải bị checkpoint hay không.

5. về cách sử dụng, edit, vận hành
      1. Để bật được file manager bạn chỉ cần nhập vào termux
      ```sh
      manager
      ```
      2. Để vận hành bot, bạn chỉ cần nhập vào termux
      ```sh
      cd ./miraiv9 && npm start
      ```

## License

This project is licensed under the GNU General Public License v3.0 License - see the [LICENSE](LICENSE) file.

<!-- CONTACT -->
## Contact
