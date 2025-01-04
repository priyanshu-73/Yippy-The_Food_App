# Yippy

Yippy is a full-stack web application for ordering food online. It consists of three main parts: the admin panel, the client-side application, and the server-side application.

## Project Structure

```
admin/
	.gitignore
	eslint.config.js
	index.html
	package.json
	public/
	README.md
	src/
		App.jsx
		assets/
		components/
		index.css
		main.jsx
		pages/
	vite.config.js
client/
	.eslintrc.cjs
	.gitignore
	index.html
	package.json
	public/
	README.md
	src/
		App.jsx
		assets/
		components/
		constants/
		context/
		index.css
		main.jsx
		pages/
	vite.config.js
server/
	.env
	.gitignore
	config/
		db.js
	controllers/
		cartController.js
		FoodController.js
		orderController.js
	middleware/
	models/
	package.json
	routes/
	server.js
	uploads/
```

## Getting Started

### Prerequisites

- Node.js
- npm or yarn
- MongoDB
- Stripe account for payment processing

### Installation

1. Clone the repository:

```sh
git clone https://github.com/your-repo/yippy.git
cd yippy
```

2. Install dependencies for each part:

```sh
# For admin
cd admin
npm install

# For client
cd ../client
npm install

# For server
cd ../server
npm install
```

3. Set up environment variables:

Create a `.env` file in the

server

directory with the following content:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
```

### Running the Application

1. Start the server:

```sh
cd server
npm run dev
```

2. Start the admin panel:

```sh
cd admin
npm run dev
```

3. Start the client-side application:

```sh
cd client
npm run dev
```

### Building for Production

1. Build the admin panel:

```sh
cd admin
npm run build
```

2. Build the client-side application:

```sh
cd client
npm run build
```

## Project Details

### Admin Panel

The admin panel is a React application built with Vite. It allows administrators to manage food items, view orders, and update order statuses.

### Client-Side Application

The client-side application is a React application built with Vite. It allows users to browse food items, add items to the cart, place orders, and view their order history.

### Server-Side Application

The server-side application is built with Express.js and MongoDB. It handles user authentication, food item management, cart management, order processing, and payment verification.

## Acknowledgements

- [React](https://reactjs.org/)
- [Vite](https://vitejs.dev/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Stripe](https://stripe.com/)
