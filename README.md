# Bedu Frontend

Dự án frontend cho hệ thống quản lý giáo dục BEDU, xây dựng bằng Next.js với App Router.

## Các thành phần chính

### Cấu trúc ứng dụng (`src/app/`)
- **(guest)/**: Các trang công khai như danh sách chương trình tự học và lớp học live.
- **manager/**: Giao diện quản trị cho quản lý tài khoản, chương trình, lớp học, bài thi, học phí và báo cáo.
- **teacher/**: Trang quản lý bài thi và lịch dạy cho giáo viên.
- **my/**: Trang cá nhân cho học viên, bao gồm khóa học, lớp học, kết quả học tập.
- **exam/**: Luồng làm bài thi với các bước chuẩn bị, thực hiện và xem kết quả.
- **auth/**: Xử lý đăng nhập và xác thực.
- **api/**: Các route API nội bộ.

### Components (`src/components/`)
- Bộ component tái sử dụng như `Button`, `Modal`, `Table`, `Breadcrumb`, `Charts`, `Input`, `Navigation`, `Sidebar`, `Tooltip`.
- Các component chuyên biệt như `LessonPreview`, `ModalClass`, `ModalCourse`, `ProgramCard`, `Question`, `Rating`, `Schedule`.

### Contexts (`src/contexts/`)
- `AppContext`: Quản lý trạng thái toàn cục của ứng dụng.
- `ExamContext`: Chia sẻ trạng thái trong luồng làm bài thi (câu hỏi, thời gian, câu trả lời).
- `MyProgramContext`: Quản lý dữ liệu chương trình của học viên.
- `TypeContext`: Định nghĩa các kiểu dữ liệu chung.

### Services (`src/services/`)
- Các hàm gọi API để tương tác với backend, như lấy danh sách chương trình, lớp học, bài thi, thanh toán.

### Types (`src/types/`)
- Định nghĩa TypeScript cho các entity như `User`, `Program`, `Class`, `Exam`, `Question`, `Payment`, `Report`.

### Helpers (`src/helpers/`)
- Các hàm tiện ích như định dạng ngày tháng (`formatDateSchedule`), định dạng tiền tệ (`formatVND`), định dạng số thứ tự (`formatNumberToOrdinal`), định dạng thời gian (`formatTime`), và lấy tên ngày đầy đủ (`getFullDayName`).

### Constants (`src/constants/`)
- Các hằng số dùng chung trong ứng dụng.

### Data (`src/data/`)
- Dữ liệu mẫu hoặc cấu hình cho các entity như class, course, exam, lesson, payment, program.

### Icons (`src/icons/`)
- Bộ icon tùy chỉnh cho ứng dụng.

### Libs (`src/libs/`)
- Các thư viện và cấu hình bổ sung, như instance Axios cho API calls.

### Providers (`src/providers/`)
- Các provider React để wrap ứng dụng, như cho authentication hoặc theme.

### Styles (`src/styles/`)
- Cấu hình styling chung.

## Công nghệ sử dụng
- **Framework**: Next.js (App Router)
- **UI Library**: NextUI
- **Styling**: Tailwind CSS
- **Data Fetching**: SWR
- **State Management**: React Context
- **Language**: TypeScript
- **HTTP Client**: Axios

## Cài đặt và chạy
1. Cài đặt dependencies: `npm install`
2. Chạy development server: `npm run dev`
3. Mở [http://localhost:3000](http://localhost:3000) để xem ứng dụng.

## Triển khai
Sử dụng Vercel hoặc các nền tảng tương thích với Next.js để triển khai production.
