# DevOps_Container2_DockerFlask
Trong Docker, mạng bridge là một loại mạng mặc định được tạo ra khi bạn cài đặt Docker trên máy tính của mình. Mạng bridge mặc định là một mạng ảo nội bộ cho phép các container trong Docker giao tiếp với nhau và với máy host. Khi bạn tạo một container mới mà không chỉ định mạng cụ thể, Docker sẽ tự động gán container đó vào mạng bridge mặc định.

Mạng bridge do người dùng tự tạo là một mạng bridge tùy chỉnh mà người dùng có thể tạo ra để đáp ứng nhu cầu đặc biệt. Bạn có thể tạo mạng bridge mới bằng Docker CLI hoặc Docker Compose và cấu hình nó theo ý muốn. Mạng bridge do người dùng tự tạo cho phép bạn tạo các mạng ảo riêng biệt để phân chia các container vào các nhóm riêng biệt hoặc tạo các mô hình mạng phức tạp hơn trong Docker.

Một số khác biệt chính giữa mạng bridge mặc định và mạng bridge do người dùng tự tạo bao gồm:

Tên: Mạng bridge mặc định có tên là bridge, trong khi mạng bridge do người dùng tự tạo có thể có tên bất kỳ.

IP Range: Mạng bridge mặc định sử dụng dải địa chỉ IP là 172.17.0.0/16, trong khi mạng bridge do người dùng tự tạo cho phép bạn định cấu hình dải địa chỉ IP tuỳ ý.

Mạng: Mạng bridge mặc định sử dụng phương pháp NAT (Network Address Translation) để cho phép các container trong mạng bridge kết nối với mạng ngoại vi. Trong khi đó, mạng bridge do người dùng tự tạo cũng có thể được cấu hình để sử dụng chế độ NAT hoặc không sử dụng NAT.

Cấu hình: Mạng bridge mặc định không yêu cầu bất kỳ cấu hình bổ sung nào. Trong khi mạng bridge do người dùng tự tạo cho phép bạn tuỳ chỉnh các cấu hình như địa chỉ IP, subnet mask, gateway, DNS, v.v.

Phạm vi truy cập: Mạng bridge mặc định chỉ cho phép các container trên cùng mạng bridge mặc định truy cập lẫn nhau và với máy host. Trong khi mạng bridge do người dùng tự tạo cho phép bạn tạo các mạng riêng biệt và kiểm soát phạm vi truy cập giữa các mạng khác nhau.
