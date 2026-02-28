# Skill: App Builder
Main application building orchestrator.  
Creates full-stack applications from natural language requests.

---

## Purpose
- Analyze user request
- Determine project type
- Select tech stack
- Plan project structure
- Coordinate agents for execution

Acts as the central orchestrator for building apps.

---

## Selective Reading Rule
Only read files relevant to the current request.  

| File | Description | When to Read |
|------|------------|--------------|
| project-detection.md | Keyword matrix, project type detection | Starting new project |
| tech-stack.md | Default stack & alternatives | Choosing tech |
| agent-coordination.md | Agent pipeline & execution | Multi-agent coordination |
| scaffolding.md | Directory structure & core files | Creating project structure |
| feature-building.md | Feature analysis & error handling | Adding new features |
| templates/SKILL.md | Project templates | Scaffold new project |

---

## Templates

Read only the matching template for the project type.

| Template | Tech Stack | Use Case |
|----------|------------|---------|
| nextjs-fullstack | Next.js + Prisma | Full-stack web app |
| nextjs-saas | Next.js + Stripe | SaaS product |
| nextjs-static | Next.js + Framer | Landing page |
| nuxt-app | Nuxt 3 + Pinia | Vue full-stack app |
| express-api | Express + JWT | REST API |
| python-fastapi | FastAPI | Python API |
| react-native-app | Expo + Zustand | Mobile app |
| flutter-app | Flutter + Riverpod | Cross-platform mobile |
| electron-desktop | Electron + React | Desktop app |
| chrome-extension | Chrome MV3 | Browser extension |
| cli-tool | Node.js + Commander | CLI app |
| monorepo-turborepo | Turborepo + pnpm | Monorepo |

---

## Related Agents

| Agent | Role |
|-------|-----|
| project-planner | Task breakdown, dependency graph |
| frontend-specialist | UI components, pages |
| backend-specialist | API, business logic |
| database-architect | Schema, migrations |
| devops-engineer | Deployment & preview |

---

## App Builder Workflow

1. **Project Type Detection**  
   Determine app type based on user description.

2. **Tech Stack Selection**  
   Pick default stack or alternatives based on project type.

3. **Project Planning**  
   - Database schema  
   - API routes  
   - Pages & routes  
   - Components & modules

4. **Scaffold Project**  
   - Create directory structure  
   - Generate core files

5. **Feature Implementation**  
   - Analyze features  
   - Assign tasks to agents  
   - Monitor progress

6. **Preview & Verify**  
   - Start local or cloud preview  
   - Report completion

---

## Usage Example

**User Request:**  
"Make an Instagram clone with photo sharing and likes"

**App Builder Actions:**

1. Project type → Social Media App  
2. Tech stack → Next.js + Prisma + Cloudinary + Clerk  
3. Plan creation:  
   - Database: users, posts, likes, follows  
   - API: 12 endpoints  
   - Pages: feed, profile, upload  
   - Components: PostCard, Feed, LikeButton  
4. Coordinate agents  
5. Report progress  
6. Start preview

---

## Notes

- Always load required agents for tasks.  
- Only scaffold or read files relevant to request.  
- For multi-agent coordination, orchestrator ensures order.  
- Keep workflow consistent for all project types.