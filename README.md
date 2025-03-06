# Ticketing System Frontend

This is the frontend for a Ticketing System built with React, TypeScript, TailwindCSS, and React Query. The application allows users to create, view, and manage tickets. It includes role-based access control, where users can be either `admin` or `user`. Admins have additional privileges, such as updating ticket statuses.

## Features

- **User Authentication**: Login and Signup functionality with role-based access control.
- **Ticket Management**:
  - Users can create and view their tickets.
  - Admins can view all tickets and update their statuses.
- **Role-Based Access Control**:
  - `Admin`: Can view all tickets and update their statuses.
  - `User`: Can create and view their own tickets.
- **Responsive Design**: Built with TailwindCSS for a responsive and modern UI.
- **State Management**: Uses React Query for efficient data fetching and caching.

## Technologies Used

- **React**: A JavaScript library for building user interfaces.
- **TypeScript**: A typed superset of JavaScript for better developer experience.
- **TailwindCSS**: A utility-first CSS framework for rapid UI development.
- **React Query**: A data-fetching library for managing server state in React applications.
- **React Router**: A library for routing and navigation in React applications.
- **HeadlessUI**: A set of completely unstyled, fully accessible UI components.
- **Axios**: A promise-based HTTP client for making API requests.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/ticketing-system-fe.git
   cd ticketing-system-fe
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Run the development server**:
   ```bash
   npm start
   ```

4. **Open the application**:
   Visit `http://localhost:3000` in your browser.

## Project Structure

```
ticketing-system-fe/
├── public/                  # Static assets
├── src/
│   ├── components/          # Reusable components
│   ├── pages/               # Page components
│   ├── services/            # API service layer
│   ├── App.tsx              # Main application component
│   ├── index.tsx            # Entry point
│   └── ...                  # Other configuration files
├── package.json             # Project dependencies
├── tailwind.config.js       # TailwindCSS configuration
└── README.md                # Project documentation
```

## Available Scripts

- **`npm start`**: Runs the app in development mode.
- **`npm test`**: Launches the test runner.
- **`npm run build`**: Builds the app for production.
- **`npm run eject`**: Ejects the app from Create React App configuration.

## Environment Variables

To run this project, you will need to set up the following environment variables in a `.env` file:

```env
REACT_APP_API_URL=http://localhost:5000/api
```

Replace `http://localhost:5000/api` with the URL of your backend API.

## API Service

The frontend interacts with the backend via the `apiService` module, which is located in `src/services/api.ts`. This module handles all API requests, including authentication, ticket creation, and ticket management.

## Protected Routes

The application uses protected routes to ensure that only authenticated users can access certain pages. The `ProtectedRoute` component checks the user's role and redirects them to the appropriate dashboard (`/admin` or `/user`).

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeatureName`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeatureName`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [React](https://reactjs.org/)
- [TailwindCSS](https://tailwindcss.com/)
- [React Query](https://tanstack.com/query/v4)
- [HeadlessUI](https://headlessui.com/)
- [Axios](https://axios-http.com/)

---

For any questions or issues, please open an issue on the GitHub repository.
