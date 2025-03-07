#





#### Design Plan

1. System Design with the following in mind
- Go-based API + game engine service manager with websockets/gRPC
- gpu inference/MCTS python service (Can I move MCTS onto the gpu to save cpu and make it much faster?)
- PostgreSQL and maybe Redis for pub/sub?
- Draw designs
2. Build without scalability
- Clone Game Engine from my github into the project
- Create basic API with Go for user information.
- Write Go service with Websocket connections
- Protobuf stuff for server - engine communication
- Write super basic frontend
3. Containerize with Docker.
- Containerize the 3/4 components 
- Test with Docker Compose
4. Intergrate Redis if needed
5. Kubernetes
