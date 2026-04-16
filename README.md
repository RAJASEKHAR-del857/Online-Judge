
# Online Judge System

## Features
- Multi-language support (C++, Python)
- Docker sandbox execution
- Redis queue
- Worker-based scalable architecture
- Time limit enforcement
- Basic verdict system (AC, CE, RE)

## Architecture
Client -> Express Server -> Redis Queue -> Worker -> Docker Execution

## Setup

### Start everything
docker-compose up --build

### API
POST /submit
{
  "code": "...",
  "lang": "cpp",
  "input": "2 3"
}

## HIGHLIGHTS
- Scalable queue system using Redis
- Secure execution via Docker isolation
- Worker horizontal scaling possible
- Language abstraction layer
