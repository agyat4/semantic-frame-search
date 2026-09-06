# Phase 1: Local Project Foundation

## Decisions

- Project name: SemanticFrameSearch
- Local directory: semantic-frame-search
- Git branch: main
- Python source location: src/semantic_frame_search
- Runtime files remain outside version control
- Search results are separated by run
- Evaluation data is separated from ordinary search results
- Robotics-part collection is the first use case, not the system boundary

## Directory responsibilities

### configs

Reusable model, sampling, scoring and deduplication settings.

### inputs

Video URL lists and structured search requests.

### data/videos

Downloaded source videos.

### data/frame_cache

Temporary frames used during video indexing.

### data/embedding_cache

Reusable SigLIP2 frame embeddings.

### data/captions

Generated captions for selected candidate frames.

### outputs/search_runs

Final extracted images and associated metadata.

### evaluation

Manually verified annotations, test queries and evaluation results.

### src/semantic_frame_search

The main Python package.

### tests

Automated and end-to-end tests.

### docs

Design decisions and implementation documentation.

## Phase 1 completion checklist

- [x] Project folder created
- [x] General project name selected
- [x] Local Git repository initialized
- [x] Main branch selected
- [x] Project directories created
- [x] Runtime data separated from source code
- [x] Generated files excluded from Git
- [x] Project purpose documented
- [ ] Dependencies selected
- [ ] Python environment created
- [ ] GitHub repository connected
- [ ] First commit created
