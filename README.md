# MCP Gemini Google Search Integration Server 🌐🔍

![MCP Server](https://img.shields.io/badge/MCP%20Server-mcp--gemini--google--search-blue)

## Overview

The **MCP Gemini Google Search** project provides a server for integrating Google Search capabilities using Gemini's built-in search features. This server allows developers to harness the power of Google's search engine within their applications, enhancing user experience and providing robust search functionality.

## Features

- **Easy Integration**: Seamlessly connect Google Search with your applications.
- **Built-in Capabilities**: Utilize Gemini's features for efficient search operations.
- **Customizable**: Tailor the search experience to fit your application's needs.
- **Scalable**: Designed to handle varying loads, from small applications to large-scale systems.

## Topics

- mcp-server

## Getting Started

To get started with the MCP Gemini Google Search server, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Chauhan901/mcp-gemini-google-search.git
   cd mcp-gemini-google-search
   ```

2. **Download the Latest Release**:
   Visit the [Releases section](https://github.com/Chauhan901/mcp-gemini-google-search/releases) to download the latest version. You will find a file that needs to be downloaded and executed.

3. **Install Dependencies**:
   Ensure you have the necessary dependencies installed. You can find them in the `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```

4. **Configuration**:
   Update the configuration file to include your Google API credentials. Make sure to follow the guidelines provided in the `CONFIG.md` file.

5. **Run the Server**:
   Start the server with the following command:
   ```bash
   python app.py
   ```

6. **Access the API**:
   Once the server is running, you can access the API at `http://localhost:5000/api`.

## API Documentation

The MCP Gemini Google Search server provides a RESTful API. Below are the main endpoints:

### Search Endpoint

- **GET** `/search`
  - **Description**: Search for a query using Google Search.
  - **Parameters**:
    - `query`: The search term.
    - `limit`: Number of results to return (optional).
  
  - **Example**:
    ```bash
    curl "http://localhost:5000/search?query=example&limit=10"
    ```

### Status Endpoint

- **GET** `/status`
  - **Description**: Check the server status.
  
  - **Example**:
    ```bash
    curl "http://localhost:5000/status"
    ```

## Configuration

The server requires a configuration file. Here's how to set it up:

1. Create a file named `config.json` in the root directory.
2. Add the following structure:
   ```json
   {
       "google_api_key": "YOUR_API_KEY",
       "google_search_engine_id": "YOUR_SEARCH_ENGINE_ID"
   }
   ```

3. Replace `YOUR_API_KEY` and `YOUR_SEARCH_ENGINE_ID` with your actual credentials.

## Example Usage

Here’s a quick example of how to use the server to perform a search:

1. Start the server.
2. Open your terminal and run the following command:
   ```bash
   curl "http://localhost:5000/search?query=hello"
   ```

3. You should receive a JSON response with search results.

## Contributing

We welcome contributions to the MCP Gemini Google Search project. To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/YourFeature
   ```
5. Create a pull request.

## Issues

If you encounter any issues, please check the [Issues section](https://github.com/Chauhan901/mcp-gemini-google-search/issues) of the repository. You can also report new issues there.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Support

For support, please visit the [Releases section](https://github.com/Chauhan901/mcp-gemini-google-search/releases) to find the latest updates and downloads.

## Additional Resources

- [Gemini Documentation](https://www.gemini.com/docs)
- [Google Search API](https://developers.google.com/custom-search/v1/overview)

## Acknowledgments

Thanks to the contributors and the community for making this project possible. Your support and feedback are invaluable.

![MCP Server](https://img.shields.io/badge/MCP%20Server-mcp--gemini--google--search-blue) 

For more information and updates, please check the [Releases section](https://github.com/Chauhan901/mcp-gemini-google-search/releases).