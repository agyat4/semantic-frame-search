# SemanticFrameSearch

SemanticFrameSearch is a local, open-source pipeline for finding useful video
frames using natural-language queries.

The first application is collecting clear images of robotics and laboratory
components from YouTube videos. However, the system is designed to remain
domain-independent.

## Version 0 inputs

- A list of YouTube video URLs
- Object names or aliases
- Acceptable situations or contexts
- Optional visibility requirements

## Version 0 outputs

- Ranked original-resolution frames
- Source video URL
- Video timestamp
- Visual similarity score
- Generated caption
- Caption-query similarity score
- Final ranking score
- Search-run metadata

## Planned pipeline

1. Download and register videos.
2. Sample video frames coarsely.
3. Retrieve candidates using SigLIP2.
4. Search promising temporal regions more densely.
5. remove temporal and visual duplicates.
6. Generate neutral captions using Florence-2.
7. Compare captions with the original query.
8. Combine visual and caption scores.
9. Extract original-resolution frames.
10. Export images and metadata.

