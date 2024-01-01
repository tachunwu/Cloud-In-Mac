# Cloud In Mac

# Basic Stack
* Orbstack: Mock kubernetes
* Distributed File System: N3 (NATS-based S3 Object Store)
* Stream Pool, Meta Server (3 Pod, Raft Algorithm)
* NEON (Serverless Postgres Database)
* Materialize Pool (Postges -> Analytical DBMS?)
* Ray (Machine Learning Platform used by Open.AI)
* ReadySet Pool
* DuckDB Pool
* Malloy (End-User: Data Scientist)
* Databend (Snowflake Alternative, benchmark is Fast, same Level as DuckDB ClickHouse)
* Stateless-based Index Service (Pull from Stream Systems)
* TigerBeetle (Need Special State Machine Design - Maybe a Good Idea for a M.S. Paper!)
* Machine Learning Model serve (mlx, tinygrad, Python API)
* MicroVM (Run for serverless function, Firecracker, Kata Containerm, unikernel)

# Database
* ScyllaDB (zig build)
* TigerBeetle (Custom State Machine)
* CockroachDB (Fair to say that CRDB is the Most advanced Distributed SQL in 2024)

# Algorithm
* Weaver Routing ->  Embedded Cache, Distributed
* Stream Cluster API Server (worker use Watch method) -> ctrl stream cluster to collect Events
* Event -> Object (csv ...etc)
* Replay Stream -> Build Index (Full-text Index, LLM /read Chain of Thought Paper/, Geo Index)
* Epoxy (State-of-the-Art Heterogenous Distributed Transaction, can be build by NATS?)
* Workflow Framework
* Hashicorp Serf
* Anything about Messaging (Canary Request, Partition, Replication)
