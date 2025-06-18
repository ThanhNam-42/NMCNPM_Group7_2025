# 🛒 Hệ thống Kinh doanh Thiết bị Điện tử - RockerShop

![Java](https://img.shields.io/badge/Java-17+-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.1+-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-15+-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-4.8+-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0+-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=for-the-badge&logo=intellij-idea&logoColor=white)

## 📋 Mục tiêu dự án

### 🎯 Mục tiêu chính
Xây dựng một **hệ thống website bán hàng thiết bị điện tử** đầy đủ chức năng, an toàn, có khả năng mở rộng, mang lại trải nghiệm mua sắm tiện lợi cho người dùng và quản lý hiệu quả cho người bán.

### 🎯 Mục tiêu cụ thể
- ✅ **Nâng cao trải nghiệm khách hàng**: Giao diện thân thiện, tốc độ tải nhanh
- ✅ **Cải thiện hiệu quả quản lý**: Quản lý sản phẩm, đơn hàng, người dùng
- ✅ **Đảm bảo an toàn**: Bảo mật thông tin và giao dịch
- ✅ **Khả năng mở rộng**: Kiến trúc linh hoạt, dễ phát triển

## 🏗️ Kiến trúc hệ thống

### 📐 Mô hình kiến trúc: Multi-tier Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    PRESENTATION TIER                        │
│                   (Angular Frontend)                       │
│  ┌─────────────┐ ┌─────────────┐ ┌─────────────┐          │
│  │ Components  │ │  Services   │ │   Guards    │          │
│  └─────────────┘ └─────────────┘ └─────────────┘          │
└─────────────────────────────────────────────────────────────┘
                              │
                         HTTP/REST API
                              │
┌─────────────────────────────────────────────────────────────┐
│                  BUSINESS LOGIC TIER                       │
│                  (Spring Boot Backend)                     │
│  ┌─────────────┐ ┌─────────────┐ ┌─────────────┐          │
│  │ Controllers │ │  Services   │ │ Repositories│          │
│  └─────────────┘ └─────────────┘ └─────────────┘          │
└─────────────────────────────────────────────────────────────┘
                              │
                          JPA/Hibernate
                              │
┌─────────────────────────────────────────────────────────────┐
│                      DATA TIER                             │
│                    (MySQL Database)                        │
└─────────────────────────────────────────────────────────────┘
```

### 🔄 Hướng phát triển: API-driven Development
- **Frontend (SPA)**: Angular Application với giao tiếp qua HTTP
- **Backend (API)**: Spring Boot RESTful API Server
- **Giao tiếp phi trạng thái**: Stateless Communication

## 🛠️ Công nghệ sử dụng

### 🖥️ Backend Technologies
- **Java 17+** - Ngôn ngữ lập trình chính
- **Spring Boot 3.1+** - Framework chính cho backend
- **Spring Data JPA** - Lớp trừu tượng cho database operations
- **Spring Security** - Xác thực và phân quyền
- **MySQL 8.0+** - Hệ quản trị cơ sở dữ liệu

### 🌐 Frontend Technologies  
- **Angular 15+** - Framework chính cho SPA
- **TypeScript 4.8+** - Ngôn ngữ lập trình frontend
- **Angular CLI** - Công cụ phát triển Angular
- **HTML5 & CSS3** - Markup và styling
- **Bootstrap/Angular Material** - UI Components

### 🔧 Development Tools
- **IntelliJ IDEA** - IDE chính cho phát triển
- **Node.js & npm** - Quản lý packages frontend
- **Git** - Version control system
- **Maven/Gradle** - Build tool cho Java

## ✨ Tính năng hệ thống

### 🎯 Giai đoạn 1 (Hoàn thành)
- ✅ **Xác thực người dùng**: Đăng ký/đăng nhập với JWT
- ✅ **Quản lý sản phẩm**: CRUD operations cho admin
- ✅ **Hiển thị sản phẩm**: Danh sách và chi tiết sản phẩm
- ✅ **Giỏ hàng**: Thêm sản phẩm và đặt hàng cơ bản
- ✅ **Admin Panel**: Giao diện quản trị

### 🚀 Giai đoạn 2 (Mở rộng)
- 🔄 **Thanh toán trực tuyến**: Tích hợp payment gateway
- 🔄 **Tìm kiếm nâng cao**: Bộ lọc và search functionality
- 🔄 **Quản lý đơn hàng**: Tracking và status management
- 🔄 **Đánh giá sản phẩm**: Review và rating system
- 🔄 **Phân quyền**: Role-based access control

### 📊 Admin Panel Features
- 📱 **Quản lý sản phẩm**: Thêm/sửa/xóa thiết bị điện tử
- 👥 **Quản lý khách hàng**: Thông tin và lịch sử mua hàng
- 🛒 **Quản lý đơn hàng**: Xử lý và cập nhật trạng thái
- 📈 **Dashboard**: Thống kê doanh thu và báo cáo
- ⭐ **Quản lý đánh giá**: Moderation của review
- 📊 **Phân tích**: Insights về sản phẩm bán chạy

## 🚀 Cài đặt và Triển khai

### 📋 Yêu cầu hệ thống
- **Java 17+**
- **Node.js 16+** 
- **MySQL 8.0+**
- **Maven 3.8+**
- **Angular CLI 15+**


## 📁 Cấu trúc dự án

### 🖥️ Backend Structure
```
src/main/java/
├── controller/          # REST Controllers
├── service/            # Business Logic Layer
├── repository/         # Data Access Layer
├── entity/            # JPA Entities
├── dto/               # Data Transfer Objects
├── config/            # Configuration Classes
└── security/          # Security Configuration
```

### 🌐 Frontend Structure
```
src/app/
├── admin/                 # Admin Module
│   ├── dashboard/         # Dashboard Component
│   ├── product/           # Product Management
│   ├── customer/          # Customer Management
│   ├── order/             # Order Management
│   └── statistical/       # Analytics & Reports
├── common/                # Shared Models
├── services/              # Angular Services
├── guard/                 # Route Guards
└── components/            # Shared Components
```

## 🔒 Bảo mật

### 🛡️ Backend Security
- **JWT Authentication**: Stateless authentication
- **Spring Security**: Role-based access control
- **Password Encryption**: BCrypt hashing
- **API Rate Limiting**: Prevent abuse
- **Input Validation**: SQL injection prevention

### 🔐 Frontend Security
- **Route Guards**: Protect admin routes
- **HTTP Interceptors**: Automatic token handling
- **XSS Prevention**: Sanitize user inputs
- **CSRF Protection**: Cross-site request forgery prevention

## 🧪 Testing & Quality Assurance

### 🔍 Phương pháp đảm bảo chất lượng
- **Unit Testing**: JUnit (Backend), Jasmine/Karma (Frontend)
- **Integration Testing**: Test API endpoints
- **Code Review**: Peer review process
- **Version Control**: Git với branch strategy
- **Logging & Monitoring**: Application monitoring


## 🚀 Hiệu năng & Tối ưu hóa

### ⚡ Frontend Optimization
- **Lazy Loading**: Modules loaded on demand
- **AOT Compilation**: Ahead-of-Time compilation
- **Tree Shaking**: Remove unused code
- **Code Splitting**: Optimize bundle size
- **Caching Strategy**: Browser và HTTP caching

### 🏃‍♂️ Backend Optimization
- **Database Indexing**: Optimize query performance
- **Connection Pooling**: Efficient database connections
- **Caching**: Redis cho frequently accessed data
- **Query Optimization**: JPA query tuning

## 🔮 Hướng phát triển tương lai

### 🎯 Tính năng mới
- 🤖 **AI Chatbot**: Hỗ trợ khách hàng tự động
- 🧠 **Recommendation System**: AI-powered product suggestions
- 📱 **Mobile App**: React Native/Flutter app
- 🌐 **Multi-language**: Internationalization support
- 📊 **Advanced Analytics**: Business intelligence dashboard

### 🛠️ Cải tiến kỹ thuật
- ☁️ **Cloud Deployment**: AWS/Azure deployment
- 🐳 **Containerization**: Docker & Kubernetes
- 🔄 **CI/CD Pipeline**: Automated deployment
- 📈 **Microservices**: Service-oriented architecture
- 🗄️ **Database Optimization**: Sharding và replication

## 🤝 Đóng góp

### 📋 Coding Standards
- **Backend**: Google Java Style Guide
- **Frontend**: Angular Style Guide
- **Database**: Naming conventions
- **Documentation**: Javadoc và TSDoc


## 📞 Liên hệ & Hỗ trợ

- 👨‍💻 **Developer**: Nguyễn Thành Nam - Trương Tuấn Huy
- 🏫 **Institution**: [Học viện Công nghệ Bưu chính viễn thông - PTIT/Khoa Công nghệ thông tin 2]
- 📧 **Email**: ntnam.rock@gmail.com
- 📱 **Phone**: +84 339110261

## 📚 Tài liệu tham khảo

- [Spring Boot Documentation](https://spring.io/projects/spring-boot)
- [Angular Documentation](https://angular.io/docs)
- [MySQL Documentation](https://dev.mysql.com/doc/)
- [Spring Security Reference](https://spring.io/projects/spring-security)
- [Angular Style Guide](https://angular.io/guide/styleguide)


<div align="center">

**🌟 Hệ thống Kinh doanh Thiết bị Điện tử 🌟**

*Xây dựng với ❤️ bằng Spring Boot & Angular*

[![Made with Java](https://img.shields.io/badge/Made%20with-Java-ED8B00.svg)](https://www.java.com)
[![Made with Angular](https://img.shields.io/badge/Made%20with-Angular-DD0031.svg)](https://angular.io)
[![Made with Spring Boot](https://img.shields.io/badge/Made%20with-Spring%20Boot-6DB33F.svg)](https://spring.io/projects/spring-boot)

</div>
