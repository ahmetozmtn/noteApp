##language options
- [Turkish](#Turkish)

- 
## Start
User Note Taking Application (API Only)

This project is an API-based user system and note-taking application where users can log in, register, update their information, and add notes. The project also includes an admin system for managing user-related operations.

Users are provided with a simple log system that records their actions, no matter how basic they may be.

At this stage, there is no frontend part available.
You can run the project on your local machine by following the steps below:

1. Clone this project by running the following command:
git clone https://github.com/melihAkn/noteApp

2. Navigate to the project folder:
cd .\noteApp\Backend\

3. Install the required dependencies by running the following command:
npm install

4. Start the MongoDB database:
mongod

5. Run the project by executing the following command:
npm start

6. You can use an API development tool (such as Postman, cURL, etc.) to test the APIs.

## API Documentation

The project's APIs work with JWT-based authentication. The following APIs are available:

- `POST http://localhost:3000/users/signup`: To create a new user registration, you can use the following API endpoint. The required parameters are:`name`, `surName`, `email`,`userName`,`password`.

- `POST http://localhost:3000/users/login`: It is used for user login. The required parameters are username or email and password.The required parameters are:`email` or `userName`,`password`. Upon successful login, a JWT token is returned.

- `POST http://localhost:3000/users/addNote`: It retrieves the profile information of the current user. A valid JWT token is required for authentication.

- `GET http://localhost:3000/users/myNotes`: It allows retrieving the notes added by the current user in the system. A valid JWT token is required for authentication.The required parameters are:`userNotes`

- `PATCH http://localhost:3000/users/user`: It allows the user to update their own information. A valid JWT token is required for authentication.

------------------------------Admin operations-------------------------------------
- `GET http://localhost:3000/admin`: When accessing the admin homepage, it returns the value "Welcome".

- `POST http://localhost:3000/admin/login`: It is used for admin login. The required parameters are username and password.The required parameters are:`userName`,`password`. Upon successful login, a JWT token is returned.

- `POST http://localhost:3000/admin/register`: It is used to create a new admin record. The required parameters are `userName`,`password`.

- `PATCH http://localhost:3000/admin/update`: It is used to update the information of an admin in the system.

Admin can perform various operations related to users.

- `GET http://localhost:3000/admin/getUsers`: To retrieve all users, an admin can make use of the following operation. A valid JWT token is required for authentication.

- `GET http://localhost:3000/admin/getUser`: To retrieve a user based on their username, an admin can use the following operation.The required parameters are `userName`. A valid JWT token is required for authentication.

- `DELETE http://localhost:3000/admin/deleteUser`: To delete a user based on their username or email, an admin can use the following operation.The required parameters are `userName` or `email`. A valid JWT token is required for authentication.

- `DELETE http://localhost:3000/admin/deleteUser`: To delete a user based on their username or email, including the deletion of their associated notes, an admin can use the following operation.The required parameters are `userName` or `email`. A valid JWT token is required for authentication.

- `GET http://localhost:3000/admin/deleteAllUser`: To delete all users and their associated notes, an admin can use the following operation. A valid JWT token is required for authentication.
- 
When making requests to API endpoints, you should send the data in JSON format.
For more details, you can review the source code of the project.
## Contributions and License
This project is open source and welcomes contributions and suggestions from the community.

## Turkish

# Kullanıcı Not Alma Uygulaması (Sadece API)

Bu proje, kullanıcıların sisteme giriş yapabileceği, kayıt olabileceği, bilgilerini güncelleyebileceği ve notlarını ekleyebileceği bir kullanıcı sistemi ve not alma uygulaması ve kullanıcılar sadece API kısmını içermektedir ve ayrıca kullanıcılar ile ilgili işlemler için admin sistemini içermektedir.

kullanıcılar herhangi bir işlem yaptıgında her ne kadar basitte olsa yaptıkları işlem ile alakali bir log sistemi vardir.

Bu aşamada herhangi bir frontend kısmı bulunmamaktadır.

## Başlangıç

Aşağıdaki adımları izleyerek projeyi yerel makinenizde çalıştırabilirsiniz:

1. Bu projeyi kopyalamak için aşağıdaki komutu çalıştırın:
git clone https://github.com/melihAkn/noteApp

2. Proje klasörüne gidin:
cd .\noteApp\Backend\

3. Gerekli bağımlılıkları yüklemek için aşağıdaki komutu çalıştırın:
npm install

4. MongoDB veritabanını başlatın:
mongod

5. Projeyi başlatmak için aşağıdaki komutu çalıştırın:
npm start

6. API'ları test etmek için bir API geliştirme aracı (Postman, cURL vb.) kullanabilirsiniz.

## API Dökümantasyonu

Projenin API'ları JWT tabanlı kimlik doğrulama ile çalışır. Aşağıdaki API'lar mevcuttur:

- `POST http://localhost:3000/users/signup`: Yeni bir kullanıcı kaydı oluşturmak için kullanılır. İstenen parametreler: `name`, `surName`, `email`,`userName`,`password`.

- `POST http://localhost:3000/users/login`: Kullanıcı girişi yapmak için kullanılır. İstenen parametreler: `username` or `email`, `password`. Başarılı giriş sonrası, bir JWT token döner.

- `POST http://localhost:3000/users/addNote`: Mevcut kullanıcının profil bilgilerini getirir. Kimlik doğrulama için geçerli bir JWT token gereklidir.

- `GET http://localhost:3000/users/myNotes`: Mevcut kullanıcının sisteme eklediği notları getirmesini sağlar. Kimlik doğrulama için geçerli bir JWT token gereklidir.

- `PATCH http://localhost:3000/users/user`: Kullanıcının kendi bilgilerini guncellemesini sağlar. Kimlik doğrulama için geçerli bir JWT token gereklidir. 

------------------------------ADMİN İSLEMLERİ-------------------------------------
- `GET http://localhost:3000/admin`: admin ana sayfasına girildiğinde "hoşgeldiniz" degerini dondurur.

- `POST http://localhost:3000/admin/login`: admin girişi yapmak için kullanılır. İstenen parametreler: `username`, `password`. Başarılı giriş sonrası, bir JWT token döner.

- `POST http://localhost:3000/admin/register`: Yeni bir admin kaydı oluşturmak için kullanılır. İstenen parametreler: `userName`,`password`.

- `PATCH http://localhost:3000/admin/update`: adminin sistemdeki bilgilerini guncellemesi icin kullanılır.

ADMİNİN KULLANICILAR İLE İLGİLİ YAPACAGI İŞLEMLER
- `GET http://localhost:3000/admin/getUsers`: adminin  tum lullanıcıları
getirmesini sağlar. Kimlik doğrulama için geçerli bir JWT token gereklidir.


- `GET http://localhost:3000/admin/getUser`: adminin  kullanıcı adına gore kullanıcı getirmesini sağlar. Kimlik doğrulama için geçerli bir JWT token gereklidir. istenen parametreler : `userName`

- `DELETE http://localhost:3000/admin/deleteUser`: adminin  kullanıcı adına veya emaile gore kullanıcı silmesini sağlar. Kimlik doğrulama için geçerli bir JWT token gereklidir. istenen parametreler : `userName` or `email`

- `DELETE http://localhost:3000/admin/deleteUser`: adminin  kullanıcı adına veya emaile gore kullanıcı silmesini ve silinen kullanıcının notlarınıda silmesini sağlar. Kimlik doğrulama için geçerli bir JWT token gereklidir. istenen parametreler : `userName` or `email`

- `GET http://localhost:3000/admin/deleteAllUser`: adminin tum kullanıcıları ve kullanıcıların notlarınıda silmesini sağlar. Kimlik doğrulama için geçerli bir JWT token gereklidir. istenen parametreler.
API endpoint'lerine istek yaparken JSON formatında veri göndermelisiniz.

Daha fazla detay için, projenin kaynak kodlarını inceleyebilirsiniz.

## Katkılar ve Lisans
Bu proje açık kaynaklıdır. Her türlü katkı ve öneriye açıktır.









