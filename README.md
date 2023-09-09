
# Contact Management App

Welcome to the Contact Management App! This document will guide you through the steps to set up and run the app locally.

## Backend API Setup

1. Clone the backend repository if you haven't already:

   ```bash
   git clone https://github.com/bkabhi/contact-management-app.git
   ```

2. Navigate to the backend directory:

   ```bash
   cd contact-management-app/back-end
   ```

3. Install the required dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the backend directory and set the `MONGODB_URI` to either your local development API or the deployed API. Example `.env` file for local development:

   ```
   MONGODB_URI=your-mongodb-url
   ```

5. Build and start the backend server:

   ```bash
   npm run build
   npm run start-dev
   ```

The backend API should now be running locally on `http://localhost:5000`.

## Frontend Setup

1. Clone the frontend repository if you haven't already:

   ```bash
   git clone https://github.com/bkabhi/contact-management-app.git
   ```

2. Navigate to the frontend directory:

   ```bash
   cd contact-management-app/front-end
   ```

3. Install the required dependencies:

   ```bash
   npm install
   ```

4. Open the `src` directory and locate the `rootService.ts` file. Update the `BASE_API_URL` to match the backend API URL. Example for local development:

   ```javascript
   export const BASE_API_URL = "http://localhost:5000/api";
   ```

5. Run the frontend development server:

   ```bash
   npm run dev
   ```

The frontend should now be running locally, and you can access it in your browser at `http://127.0.0.1:5173`.

## Accessing the App

- The Contact Management App should now be accessible at `http://127.0.0.1:5173`.
- You can navigate to the Contact Management and Charts & Maps pages using the paths you've defined in your routing configuration.

## API Endpoints

- The app uses the following API endpoints:
  - For contact management: `${BASE_API_URL}/contact-management-app`
  - For COVID-19 data:
    - Countries data: `https://disease.sh/v3/covid-19/countries`
    - Historical data: `https://disease.sh/v3/covid-19/historical/all?lastdays=all`

Make sure that your backend API is running and configured correctly with these endpoints for the app to work as expected.

Now you should have the Contact Management App up and running locally with the provided API endpoints.
```

Feel free to customize this README to include any additional information or instructions specific to your app or development environment.