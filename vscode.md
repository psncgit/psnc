# Visual Studio Code setting

## Prerequisites
1. git-hub 계정
    - [GitHub](https://github.com/)
2. Install git-scm
    - [Git SCM](https://git-scm.com/)
3. Install Node.js
    - [Node.js](https://nodejs.org/ko/download/)
## Setup
1. Install Visual Studio Code
    - [Visual Studio Code - Code Editing. Redefined](https://code.visualstudio.com/)
2. git configuration
    ```sh
    git config --global user.name "Your Name"
    git config --global user.email you@example.com
    git config --global http.sslVerify false
    ```
3. Clone the repository and navigate into it(예스코)
    ```sh
    git clone https://github.com/psncgit/Yesco.git
    cd Yesco
    ```
4. Install all dependencies
    ```sh
    npm install
    ```
5. Start a local server and run the application (http://localhost:8080/index.html)
    ```sh
    npm start
    ```
6. Deploy the application
    ```sh
    npm run deploy
    ```