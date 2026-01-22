# Reference
<details><summary><code>client.<a href="/src/Client.ts">search</a>({ ...params }) -> tropicalia.SearchResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Perform a semantic search across project documents
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.search({
    projectId: "proj_9f8b7c6d",
    query: "Best practices for sustainable tropical agriculture",
    retrieval_strategy: "hybrid",
    expand_query: false,
    rerank: true,
    generate_answer: true,
    include_sources: true,
    limit: 50
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.SearchRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `tropicaliaClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Projects
<details><summary><code>client.projects.<a href="/src/api/resources/projects/client/Client.ts">listProjects</a>({ ...params }) -> tropicalia.Project[]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns all projects for the authenticated user
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.projects.listProjects();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.ListProjectsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ProjectsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="/src/api/resources/projects/client/Client.ts">createProject</a>({ ...params }) -> tropicalia.Project</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new project
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.projects.createProject({
    name: "Tropical Rainforest Conservation",
    description: "A project focused on preserving tropical rainforest biodiversity."
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.CreateProjectRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ProjectsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="/src/api/resources/projects/client/Client.ts">getProject</a>({ ...params }) -> tropicalia.Project</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns a specific project by ID
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.projects.getProject({
    projectId: "proj_9f8b7c6d"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.GetProjectRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ProjectsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="/src/api/resources/projects/client/Client.ts">updateProject</a>({ ...params }) -> tropicalia.Project</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update a project by ID
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.projects.updateProject({
    projectId: "proj_9f8b7c6d",
    name: "Tropical Rainforest Conservation",
    description: "A project focused on preserving the biodiversity of tropical rainforests."
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.UpdateProjectRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ProjectsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="/src/api/resources/projects/client/Client.ts">deleteProject</a>({ ...params }) -> tropicalia.ProjectDeleteResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a project and all its documents
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.projects.deleteProject({
    projectId: "proj_9f8d7c2a"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.DeleteProjectRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ProjectsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Upload
<details><summary><code>client.upload.<a href="/src/api/resources/upload/client/Client.ts">file</a>({ ...params }) -> tropicalia.UploadResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Upload a file for processing and indexing. Max 100MB.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.upload.file({
    file: fs.createReadStream("/path/to/your/file"),
    projectId: "projectId"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.UploadFileRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `UploadClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.upload.<a href="/src/api/resources/upload/client/Client.ts">listDocuments</a>({ ...params }) -> tropicalia.Document[]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List all documents in a project
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.upload.listDocuments({
    projectId: "proj_9f8b7c6d5e4a3b2c1d0e"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.ListDocumentsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `UploadClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.upload.<a href="/src/api/resources/upload/client/Client.ts">deleteDocument</a>({ ...params }) -> tropicalia.DocumentDeleteResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a document from the project
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.upload.deleteDocument({
    projectId: "proj_9f8b7c6d5e4a3b2c1d0e",
    documentId: "3fa85f64-5717-4562-b3fc-2c963f66afa6"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `tropicalia.DeleteDocumentRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `UploadClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>
