FROM node:18.9.1

WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of your app's source code
COPY . .

# Expose the port Vite will use
EXPOSE 5173

# Use npx to run vite
CMD ["npx", "vite", "--host", "0.0.0.0"]
