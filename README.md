## 🚀 How to Run Locally

1. Clone the repo
   git clone https://github.com/github-1703/your-repo-name.git

2. Setup the database

   mysql -u root -p -e "CREATE DATABASE hospital_db";
                    
   mysql -u root -p hospital_db < db/schema.sql

   mysql -u root -p hospital_db < db/procedures.sql

   mysql -u root -p hospital_db < db/triggers.sql

   mysql -u root -p hospital_db < db/views.sql

   mysql -u root -p hospital_db < db/seed.sql

3. Create backend/.env file

   DB_HOST=localhost

   DB_USER=root

   DB_PASSWORD=your_mysql_password

   DB_NAME=hospital_db

   PORT=3000

4. Install dependencies and start

   cd backend

   npm install
   
   npm run dev

5. Open http://localhost:3000 in your browser