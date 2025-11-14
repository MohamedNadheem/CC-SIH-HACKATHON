# CC-SIH-HACKATHON
# Smart India Hackathon Workshop
# Date: 18:11:2025
## Register Number:212223240091
## Name:M0HAMED NADHEEM N

## Problem Title 


E-Waste Facility Locator
## Problem Description
Website that tells you the location of the nearest e-waste collection and recycling facility. Offers educational pop-ups on the harmful components of your e-waste and their effects on the environment and human health if not disposed correctly. There could be an option to input the model of your old device and earn credit points relative to the amount of precious metals recovered from the device if disposed correctly.
## Problem Creater's Organization
Ministry of Environment

## Idea
Interactive 3D Models

Realistic 3D plant models (GLTF/GLB) with level-of-detail (LOD) for performance.

Pan, rotate, zoom, and explode-view (roots, leaves, flowers) controls.

Hotspots on plant parts to show medicinal uses, active constituents, and harvest timing.

Detailed Information Pages

Botanical name, common names, family, habitat, distribution map, cultivation practices, pharmacological uses, contraindications, parts used (leaf/root/flower), dosage forms, and references.

Multimedia Integration

High-resolution images, short educational videos, audio narration (regional languages), and downloadable PDFs.

Search & Filter

Full-text search + filters: AYUSH system (Ayurveda/Unani/Siddha/Homeopathy), medicinal use (digestive, respiratory, immunity...), region/habitat, plant type (herb/shrub/tree), flowering season, conservation status.

Virtual Tours & Thematic Trails

Pre-built guided tours (e.g., "Plants for Diabetes", "Skin Care Herbs") with narration, sequence of plants, and assessment quizzes.

User Interactions

Bookmark, annotate (notes per plant), export notes, rate plants, and share snippets to social media.

Admin & Contributor Portal

Add/edit plant entries, upload 3D models, moderate user contributions, and manage multimedia.

Offline & Accessibility

PWA caching for offline reading; text-to-speech and multilingual support; WCAG-compliant UI.

## Technical Stack

Frontend: React (Vite) + Three.js / React Three Fiber, Tailwind CSS, i18n (react-i18next)

Backend: Node.js + Express (or NestJS)

Database: PostgreSQL + PostGIS

Search: OpenSearch / Elasticsearch

Object storage: AWS S3 / MinIO

CMS: Strapi or Directus (for curated content)

Authentication: Keycloak or Firebase Auth (support social login)

3D Formats: GLTF/GLB (export from Blender)

DevOps: Docker, GitHub Actions (CI/CD), Kubernetes (optional)

Hosting: AWS / Azure / GCP or on-prem for institutions

## Data Model

Plants table

plant_id (PK)

botanical_name

common_names (array)

family

ayush_systems (array)

description

parts_used (array)

medicinal_uses (array of tags)

contraindications

cultivation_practices (text)

distribution_geojson

conservation_status

created_by, updated_by

Media table

media_id, plant_id (FK), media_type (image, video, audio, 3dmodel), url, caption, language

Users table

user_id, name, email, role (student/practitioner/admin), bookmarks (array of plant_id)

Notes table

note_id, user_id, plant_id, content, created_at

Search index

Index plant textual fields + tags + metadata for fast faceted queries




## Proposed Solution / Architecture Diagram
<img width="1536" height="1024" alt="IMG 1" src="https://github.com/user-attachments/assets/ef634b7b-a43e-46a1-b0e1-e6da695636d2" />


## Use Cases
<img width="1024" height="1024" alt="IMG 2" src="https://github.com/user-attachments/assets/67449617-2ddc-4d95-af76-775e65fdb25a" />



## Next Steps
Next Steps (What you can do now)

Fork the referenced repository and create a project board (issues for models, data, frontend, backend).

Start collecting 50 priority plants (choose from AYUSH lists) and gather images & references.

Produce 3D models for the top 10 plants 

M
