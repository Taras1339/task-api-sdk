# Task API SDK

TypeScript SDK client for the Task Management API, generated from `openapi.yaml`.

## Regenerate

    npm install
    npm run generate

## Usage

    import { client, listProjects, createTask } from "./src/client";

    client.setConfig({ baseUrl: "http://localhost:8080/v1", headers: { Authorization: "Bearer <token>" } });
    const { data } = await listProjects();
    await createTask({ path: { projectId: 1 }, body: { title: "Prepare mockups", priority: "high" } });
