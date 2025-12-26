### Project Folder
- .gitignore
- README.md
- Backend
- Frontend

### Backend Folder
- Create a blank solution (Backend)
- Add Project API (Web API) : Controller, appsettings.json, Program.cs -- Infrastructure, Application
- Add Project Infrastructure (Class Library) : Persistence (Data, Migrations), Repositories, Services -- Domain & Application
- Add Project Application (Class Library) : Interfaces (Repositories, Services), Features (Commands, Queries, DTOs) -- Domain
- Add Project Domain (Class Library) : Entities, Enums -- No Dependencies

### Frontend Folder
- Public Folder : Favicon.ico, Asserts (Images, Fonts, Icons)
- Src/app : Core (guards, interceptors, services, models), Shared (components, services, models, pipes), Features (Each folder Contains) (components, services, models, routing), layouts : (main, auth), app compoents (all 4 files, app.config, app.routes)
- src : Asserts (Images, Icons, Fonts), Environments (environment.ts, environement.deployment.ts, environment.production.ts), styles, index, main, angular.json, package-lock.json, package.json, tsconfig.app.json, tsconfig.json, tsconfig.spec.json