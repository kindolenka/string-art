
# StringArt

StringArt is a creative platform for converting photos into thread-based artwork templates. This README outlines the steps required to set up and run the project in your local development environment.

---

## System Dependencies 🛠️

Ensure you have the following installed:

- **Programming Language**: Ruby `3.1.4`
- **Framework**: Rails `7.0+`
- **Database**: PostgreSQL `>= 12.0`
- **Package Management**: Yarn `>= 1.22`
- **Node.js**: `>= 14.0`
- **Image Processing**: ImageMagick or libvips for ActiveStorage
- **Testing Frameworks**: RSpec, Capybara

---

## Getting Started 🚀

Follow these steps to set up the project locally:

### Install Dependencies  
1. **Install Ruby Gems**:  
   ```bash
   bundle install
   ```
2. **Install JavaScript Packages**:  
   ```bash
   yarn install
   ```

### Database Setup  
1. Create and configure the database:  
   ```bash
   rails db:setup
   ```
2. If needed, seed the database:  
   ```bash
   rails db:seed
   ```

### Environment Variables  
1. Copy the example environment configuration:  
   ```bash
   cp .env.example .env
   ```
2. Update `.env` with your environment-specific variables.

### Run the App Locally  
1. Start the Rails server:  
   ```bash
   rails server
   ```
2. Access the app at [http://localhost:3000](http://localhost:3000).

---

## Running Tests ✅

Run the test suite to ensure the app is working as expected:

1. **Run RSpec** (backend tests):  
   ```bash
   rspec
   ```
2. **Run Frontend Tests** (if applicable):  
   ```bash
   yarn test
   ```

---

## Deployment 📦

Use the following commands to deploy the app:

1. **Precompile Assets**:  
   ```bash
   rails assets:precompile
   ```
2. **Migrate Database**:  
   ```bash
   rails db:migrate
   ```
3. Restart your server or deployment pipeline.

---

## Monitoring & Health Check 🩺

To check the application's health, you can access the `/health` endpoint:  
```bash
curl http://localhost:3000/health
```

This will return a `200 OK` response if the app is running correctly.

---

## Additional Commands 🛡️

- **Console Access**:  
   ```bash
   rails console
   ```
- **Linting & Code Quality**:  
   ```bash
   rubocop
   ```
- **Clear Temporary Files**:  
   ```bash
   rails tmp:clear
   ```

---

Let me know if you'd like to add or modify anything!
