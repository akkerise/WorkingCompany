# Phân Tích Nghiệp Vụ Ngân Lượng Ngày 11.05.2017
### Kênh Thanh Toán : Nạp , Rút.
### Hình Thức Thanh Toán : 
* **Online** : Bank , Payment Gateway (Onepay , SmartLink , BankNet) IB , ATM_ON.
* **Offline** : 
     * Nộp tiền : quầy NL (Ngân Lượng), quầy NH (Ngân Hàng)
     * Chuyển tiền.
     * Nạp tiền : 
        1. KH tạo giao dịch với phương thức offline (login => nạp tiền).
        
            *``Tạo ra phiếu thu chưa thu tiền``*
            
        2. KH nhắn tin theo format NL về đầu số tổng đài của NL.
        
            *``Tạo ra 1 cashin notify (trạng thái hoặc thông tin của phiếu thu)``*
            
        3. Vận hành kiểm tra tiền trên hệ thống Tài Khoản Ngân Hàng . TK NL nhận tiền 
        4. Xử lý phiếu thu : chưa thu => đã thu => chuyển ngân (chỉ nhận số dư cho KH)
        
     * Thanh Toán :
        1. Khách hàng tạo đơn hầng trên **site** MC với phương thức offline
            * Đơn hàng chưa thanh toán.
            * Phiếu thu cho đơn hàng ở trạng thái chưa thu.
            
            #####```Phần còn lại nghiệp vụ giống phần Nạp Tiền```
        
     * Rút : Rút về tài khoản NH của khách :
        1. Khách hàng tạo yêu cầu rút tiền (cashout Request)
            * Tạo 1 yêu cầu rút tiền
            * Tạo 1 GD rút tiền ở trạng thái đã xác thực.
            
        2. Vận hành NL duyệt:
            * Tạo ra 1 phiếu thu (Cashout)
            * Giao dịch rút tiền trạng thái Đã Chuyển Ngân
            
            
            
* **New Offline**

** Nạp tiền 

   ![Ảnh Nạp Tiền Được Minh Họa](http://sv1.upsieutoc.com/2017/05/11/NewMethodPaymentOffline1f34e6.md.jpg)
    
** Thanh toán và Rút tiền

   ![Thanh Toán Và Rút Tiền](http://sv1.upsieutoc.com/2017/05/11/NewMethodPaymentOffline2.md.jpg)
