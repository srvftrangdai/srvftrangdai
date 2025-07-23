<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Đăng Nhập - Hệ Thống Quản Lý Đơn Hàng</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
        }
        .background-blur {
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
    </style>
</head>
<body class="bg-gray-200">
    <div class="relative min-h-screen flex items-center justify-center bg-cover bg-center bg-no-repeat" style="background-image: url('https://images.unsplash.com/photo-1553440569-b2dc59a65c63?q=80&w=2070&auto=format&fit=crop');">
        <div class="absolute inset-0 bg-black opacity-50"></div>
        
        <div class="relative w-full max-w-md p-8 space-y-6 bg-white bg-opacity-90 background-blur rounded-2xl shadow-2xl">
            <div class="text-center">
                <img src="https://i.imgur.com/vE2w9Q3.png" alt="Logo VinFast" class="w-32 mx-auto mb-4">
                <h2 class="text-2xl font-bold text-gray-800">Hệ Thống Quản Lý Đơn Hàng</h2>
                <p class="text-gray-600">Vui lòng chọn tài khoản để tiếp tục</p>
            </div>
            
            <form id="login-form" class="space-y-6">
                <div>
                    <label for="consultant-select" class="block text-sm font-medium text-gray-700">Tư Vấn Bán Hàng</label>
                    <div class="relative mt-1">
                        <span class="absolute inset-y-0 left-0 flex items-center pl-3">
                            <i class="fas fa-user text-gray-400"></i>
                        </span>
                        <select id="consultant-select" name="consultant" required
                            class="block w-full pl-10 pr-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-blue-500 focus:border-blue-500 sm:text-sm">
                            <option value="" disabled selected>-- Chọn tên của bạn --</option>
                            <!-- Tên Admin -->
                            <option value="PHẠM THÀNH NHÂN" class="font-bold text-red-600">PHẠM THÀNH NHÂN (Admin)</option>
                            <!-- Danh sách TVBH -->
                            <option value="NGUYỄN THỊ HỒNG NHUNG">NGUYỄN THỊ HỒNG NHUNG</option>
                            <option value="LÊ DƯ VĂN THÀNH">LÊ DƯ VĂN THÀNH</option>
                            <option value="NGUYỄN MINH THIỆN">NGUYỄN MINH THIỆN</option>
                            <option value="LÊ VĂN NAM">LÊ VĂN NAM</option>
                            <option value="NGUYỄN THANH CẢ">NGUYỄN THANH CẢ</option>
                            <option value="NGUYỄN MINH TRUNG">NGUYỄN MINH TRUNG</option>
                            <option value="NGUYỄN THỊ DIÊN">NGUYỄN THỊ DIÊN</option>
                            <option value="NGUYỄN BẢO XUYÊN">NGUYỄN BẢO XUYÊN</option>
                            <option value="NGUYỄN KIM HẢI">NGUYỄN KIM HẢI</option>
                            <option value="TRẦN THỊ HỒNG NHUNG">TRẦN THỊ HỒNG NHUNG</option>
                            <option value="ĐINH TÀI ĐỨC">ĐINH TÀI ĐỨC</option>
                            <option value="NGUYỄN DUY TÂN">NGUYỄN DUY TÂN</option>
                            <option value="LÊ NHỰT QUANG">LÊ NHỰT QUANG</option>
                            <option value="VŨ VIẾT HẢI">VŨ VIẾT HẢI</option>
                            <option value="NGUYỄN VĂN GIÁP">NGUYỄN VĂN GIÁP</option>
                        </select>
                    </div>
                </div>
                
                <div>
                    <button type="submit"
                        class="w-full flex justify-center py-2 px-4 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-blue-800 hover:bg-blue-900 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-700 transition duration-150 ease-in-out">
                        <i class="fas fa-sign-in-alt mr-2 mt-0.5"></i>
                        Đăng Nhập
                    </button>
                </div>
            </form>
             <p id="error-message" class="text-sm text-center text-red-600"></p>
        </div>
    </div>

    <script>
        document.getElementById('login-form').addEventListener('submit', function(event) {
            event.preventDefault();
            const consultantSelect = document.getElementById('consultant-select');
            const errorMessage = document.getElementById('error-message');
            const selectedConsultant = consultantSelect.value;

            if (selectedConsultant) {
                // Lưu tên người dùng vào sessionStorage để các trang khác có thể truy cập
                sessionStorage.setItem('currentConsultant', selectedConsultant);
                
                // Chuyển hướng đến trang quản lý chính
                window.location.href = 'yeucaughepxe.html';
            } else {
                // Hiển thị thông báo lỗi nếu chưa chọn tên
                errorMessage.textContent = 'Vui lòng chọn tên của bạn để đăng nhập.';
            }
        });
    </script>
</body>
</html>
