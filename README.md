# **SummarizeAI**

## **Introduction**

SummarizeAI is a simple web application designed to summarize articles and make them easier to read. Built using **React** and **Redux**, the application integrates with the **GPT-4 API** to provide real-time text summarization. Users can simply paste a link to an article or a body of text, and the application will generate a concise summary, saving time and effort.

## **Technologies Used**

- **React**: Used for building the user interface.
- **Redux and Redux Toolkit**: State management solution to handle application-wide data.
- **Vite**: A build tool and development server offering fast build times.
- **ESLint**: Used for maintaining code quality.
- **dotenv**: For handling environment variables.

## **Features**

- **Article Summarization**: The core functionality, allowing users to paste a link to an article for quick summarization.
- **User-Friendly Interface**: A clean and intuitive UI that streamlines the user's experience.
- **Real-time Processing**: Leveraging the GPT-4 API for quick and accurate text summarization.
- **Responsive Design**: The application is designed to be fully responsive, adapting to various screen sizes.

## **Getting Started**

### *Prerequisites*

- Node.js (v14.x or higher)
- npm (v7.x or higher)

### *Installation Steps*

1. Clone the repository to your local machine.
    ```bash
    git clone https://github.com/your-username/SummarizeAI.git
    ```
2. Navigate to the project directory.
    ```bash
    cd SummarizeAI
    ```
3. Install the required packages.
    ```bash
    npm install
    ```
4. Create a `.env` file to store your GPT-4 API key.
    ```bash
    echo "VITE_RAPID_API_ARTICLE_KEY=your-api-key-here" > .env
    ```

## **Development Setup**

### *Running Locally*

To run the project on your local machine, simply use the following command:

```bash
npm run dev
```

### *Building and Deploying*

To build the application for production, run:

```bash
npm run build
```

## **Code Structure**

The project follows a modular and maintainable code structure, making it easy to understand and contribute to. Below is an outline of the key components and their responsibilities:

- **main.jsx**: The entry point of the application where React and Redux are configured.
- **App.jsx**: The root component that hosts the `Hero` and `Demo` components.
- **Demo.jsx**: Manages the core functionality like copying, linking, and loading the summary.
- **Hero.jsx**: Primarily a presentation component likely used for a hero section.
- **article.js**: Handles API calls related to fetching and summarizing articles using Redux Toolkit.
- **store.js**: Configures the Redux store and imports `articleApi`.

## **API Integration**

The application seamlessly integrates with the GPT-4 API to provide real-time text summarization. The API is accessed via Redux Toolkit's `createApi` and `fetchBaseQuery` methods, as seen in the `article.js` file.

## **License**

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
