# AI Infrastructure Glossary

> One-line definitions for every term you'll encounter building modern AI systems.

---

## Data Infrastructure

| Term | Definition |
|------|------------|
| **Data Lake** | A centralized storage repository that holds raw data in its native format until needed. |
| **Data Warehouse** | A structured, query-optimized store for processed, historical data used in analytics and reporting. |
| **Data Mart** | A subject-specific subset of a data warehouse serving a particular team or business function. |
| **ETL** | Extract, Transform, Load — a pipeline pattern where data is transformed before being written to the destination. |
| **ELT** | Extract, Load, Transform — data is loaded raw first, then transformed inside the destination system. |
| **Data Pipeline** | An automated sequence of steps that moves and processes data from source to destination. |
| **Data Ingestion** | The process of collecting and importing raw data into a storage or processing system. |
| **Data Transformation** | Converting data from one format, structure, or schema into another to make it usable. |
| **Data Validation** | Checking data for correctness, completeness, and consistency against defined rules before use. |
| **Data Governance** | The set of policies, standards, and processes that ensure data is accurate, secure, and used responsibly. |
| **Data Lineage** | A record of data's origin and every transformation it has undergone throughout its lifecycle. |
| **Data Catalog** | A metadata inventory that helps teams discover, understand, and manage available datasets. |
| **Data Versioning** | Tracking and managing changes to datasets over time, similar to version control for code. |
| **Batch Processing** | Processing large volumes of data collected over a period of time in a single scheduled job. |
| **Stream Processing** | Processing data continuously in real time as it arrives, event by event. |
| **CDC (Change Data Capture)** | A technique that tracks and captures row-level changes in a database for downstream use. |

---

## Distributed Systems

| Term | Definition |
|------|------------|
| **Cluster** | A group of networked computers that work together as a single unified computing system. |
| **Node** | An individual machine (physical or virtual) that is part of a distributed cluster. |
| **Master Node** | The node responsible for coordinating tasks, managing state, and directing worker nodes. |
| **Worker Node** | A node that executes tasks assigned by the master node. |
| **Distributed Computing** | Solving computational problems by dividing work across multiple networked machines. |
| **Fault Tolerance** | A system's ability to continue operating correctly even when some components fail. |
| **High Availability (HA)** | A design approach that ensures a system remains operational with minimal downtime. |
| **Horizontal Scaling** | Adding more machines to a system to handle increased load (scaling out). |
| **Vertical Scaling** | Adding more CPU, RAM, or storage to an existing machine to handle increased load (scaling up). |
| **Load Balancer** | A component that distributes incoming network traffic evenly across multiple servers. |
| **Sharding** | Splitting a database or dataset into smaller, independent partitions distributed across nodes. |
| **Replication** | Copying data across multiple nodes to ensure availability and fault tolerance. |
| **Consensus** | A protocol by which distributed nodes agree on a single value or state (e.g., Raft, Paxos). |
| **Leader Election** | The process by which distributed nodes automatically choose one node to act as coordinator. |
| **Distributed Cache** | A shared in-memory data store spread across multiple nodes to speed up data access. |

---

## Cloud Infrastructure

| Term | Definition |
|------|------------|
| **IaaS** | Infrastructure as a Service — rent raw compute, storage, and networking from a cloud provider. |
| **PaaS** | Platform as a Service — a managed environment for deploying apps without managing the underlying infrastructure. |
| **SaaS** | Software as a Service — fully managed software delivered over the internet on a subscription basis. |
| **VPC** | Virtual Private Cloud — a logically isolated network within a public cloud provider's infrastructure. |
| **Subnet** | A range of IP addresses within a VPC used to segment and control network traffic. |
| **Availability Zone** | A physically separate data center within a cloud region, providing redundancy. |
| **Region** | A geographic area containing multiple availability zones where cloud resources are deployed. |
| **Object Storage** | Scalable, flat-hierarchy storage for unstructured data like files and blobs (e.g., S3, GCS). |
| **Block Storage** | Low-latency, structured storage attached to compute instances like a virtual hard drive. |
| **CDN** | Content Delivery Network — a distributed network of servers that delivers content from the closest location to the user. |
| **API Gateway** | A managed entry point that handles routing, authentication, rate limiting, and monitoring for APIs. |
| **Serverless Computing** | Running code in stateless, fully managed functions without provisioning or managing servers. |
| **Edge Computing** | Processing data closer to where it is generated (the "edge") rather than in a central data center. |

---

## Containers & Orchestration

| Term | Definition |
|------|------------|
| **Container** | A lightweight, portable unit that packages an application and its dependencies to run consistently anywhere. |
| **Docker** | The most widely used platform for building, shipping, and running containers. |
| **Docker Image** | A read-only snapshot of a container's filesystem and configuration used to create containers. |
| **Dockerfile** | A text script with instructions for building a Docker image layer by layer. |
| **Container Registry** | A storage and distribution service for Docker images (e.g., Docker Hub, ECR, GCR). |
| **Kubernetes** | An open-source container orchestration system for automating deployment, scaling, and management. |
| **Pod** | The smallest deployable unit in Kubernetes, containing one or more containers sharing network and storage. |
| **Deployment** | A Kubernetes object that declares the desired state for running a set of identical pods. |
| **ReplicaSet** | A Kubernetes controller that ensures a specified number of pod replicas are always running. |
| **StatefulSet** | A Kubernetes controller for managing stateful applications that require stable identities and persistent storage. |
| **DaemonSet** | A Kubernetes controller that ensures a pod runs on every (or selected) node in a cluster. |
| **Service** | A Kubernetes abstraction that exposes a stable network endpoint to a set of pods. |
| **Ingress** | A Kubernetes resource that manages external HTTP/S access and routing to services in the cluster. |
| **Namespace** | A virtual cluster within Kubernetes used to isolate resources and organize workloads. |
| **ConfigMap** | A Kubernetes object for storing non-sensitive configuration data as key-value pairs. |
| **Secret** | A Kubernetes object for storing sensitive data like passwords and API keys in an encoded form. |
| **Helm** | A package manager for Kubernetes that bundles resources into reusable charts. |
| **Service Mesh** | An infrastructure layer that manages service-to-service communication, security, and observability. |
| **Istio** | A popular open-source service mesh that provides traffic management, security, and telemetry for microservices. |
| **Sidecar** | A helper container deployed alongside the main container in a pod to handle cross-cutting concerns like logging or proxying. |

---

## Compute Infrastructure

| Term | Definition |
|------|------------|
| **CPU** | Central Processing Unit — the general-purpose processor that executes sequential instructions in a computer. |
| **GPU** | Graphics Processing Unit — a massively parallel processor originally for graphics, now dominant in AI training. |
| **TPU** | Tensor Processing Unit — Google's custom ASIC designed specifically for accelerating ML workloads. |
| **NPU** | Neural Processing Unit — a dedicated chip optimized for on-device AI inference tasks. |
| **Accelerator** | Any specialized hardware (GPU, TPU, NPU) designed to speed up specific computational workloads. |
| **CUDA** | NVIDIA's parallel computing platform and programming model for GPU-accelerated applications. |
| **cuDNN** | NVIDIA's GPU-accelerated library of deep learning primitives (convolutions, RNNs, etc.). |
| **Tensor Core** | A specialized processing unit inside NVIDIA GPUs that accelerates matrix multiply-accumulate operations. |
| **Memory Bandwidth** | The rate at which data can be read from or written to memory, a key bottleneck in AI workloads. |
| **VRAM** | Video RAM — dedicated high-speed memory on a GPU used to store model weights and activations during inference. |
| **Multi-GPU** | Using multiple GPUs together to train or run models that exceed single-GPU capacity or speed. |
| **Distributed GPU Cluster** | A network of machines each containing GPUs, working together on large-scale model training. |

---

## Model Training

| Term | Definition |
|------|------------|
| **Training** | The process of updating a model's parameters by minimizing loss on a dataset. |
| **Fine-tuning** | Continuing training of a pretrained model on a smaller, task-specific dataset. |
| **Pretraining** | Training a model from scratch on a large general dataset to learn broad representations. |
| **Transfer Learning** | Reusing knowledge from a model trained on one task to improve performance on a related task. |
| **Distributed Training** | Splitting the training workload across multiple GPUs or machines to reduce training time. |
| **Data Parallelism** | Distributing different batches of data across multiple devices, each holding a copy of the model. |
| **Model Parallelism** | Splitting a single large model across multiple devices because it doesn't fit on one. |
| **Pipeline Parallelism** | Splitting model layers across devices and processing micro-batches in an assembly-line fashion. |
| **Gradient** | The vector of partial derivatives indicating how much each parameter contributes to the loss. |
| **Backpropagation** | The algorithm that computes gradients by propagating the loss signal backwards through the network. |
| **Optimizer** | An algorithm (e.g., Adam, SGD) that uses gradients to update model weights during training. |
| **Learning Rate** | A hyperparameter controlling the step size of each weight update during optimization. |
| **Epoch** | One complete pass through the entire training dataset. |
| **Batch** | A subset of training data used to compute a single gradient update. |
| **Mini-Batch** | A small batch (typically 16–512 samples) used in stochastic gradient descent for efficient training. |
| **Checkpoint** | A saved snapshot of model weights at a point during training, enabling resumption or rollback. |
| **Hyperparameter** | A configuration value set before training (e.g., learning rate, batch size) that controls the training process. |
| **Hyperparameter Tuning** | Systematically searching for the hyperparameter values that produce the best model performance. |
| **Mixed Precision Training** | Using both 16-bit and 32-bit floating point numbers during training to speed up computation and reduce memory. |
| **Quantization-Aware Training** | Training a model while simulating the effects of quantization so it degrades less during post-training compression. |

---

## MLOps

| Term | Definition |
|------|------------|
| **MLOps** | A set of practices combining ML, DevOps, and data engineering to reliably deploy and maintain models in production. |
| **CI/CD** | Continuous Integration / Continuous Deployment — automated pipelines for building, testing, and deploying software. |
| **CT (Continuous Training)** | Automatically retraining models on new data as it becomes available to prevent performance degradation. |
| **Experiment Tracking** | Recording hyperparameters, metrics, and artifacts from each training run for comparison and reproducibility. |
| **Model Registry** | A centralized store for versioned, production-ready models with associated metadata and lifecycle status. |
| **Feature Store** | A centralized repository for storing, sharing, and serving computed ML features across teams and models. |
| **Feature Engineering** | Transforming raw data into informative inputs (features) that improve model performance. |
| **Feature Pipeline** | An automated workflow that computes and stores features from raw data on a schedule or trigger. |
| **Model Versioning** | Tracking different iterations of a trained model with unique identifiers and metadata. |
| **Reproducibility** | The ability to recreate an exact model training result given the same code, data, and configuration. |
| **Artifact Store** | A storage system for versioned ML artifacts such as datasets, models, and metrics. |
| **Workflow Orchestration** | Scheduling and managing the execution order and dependencies of steps in an ML pipeline. |
| **Model Lifecycle Management** | Managing a model through all stages — development, staging, production, and retirement. |

---

## Model Serving

| Term | Definition |
|------|------------|
| **Inference** | Running a trained model on new input data to generate predictions or outputs. |
| **Online Inference** | Real-time, low-latency inference triggered by individual requests as they arrive. |
| **Batch Inference** | Running inference on a large dataset offline in a single scheduled job. |
| **Real-Time Inference** | Inference with strict latency requirements, typically serving responses within milliseconds. |
| **Endpoint** | A network-accessible URL that accepts requests and returns model predictions. |
| **API Serving** | Exposing a model's inference capability through a REST or gRPC API. |
| **Autoscaling** | Automatically increasing or decreasing the number of serving replicas based on traffic load. |
| **Throughput** | The number of requests or tokens a model server can process per second. |
| **Latency** | The time elapsed from sending a request to receiving the model's response. |
| **Cold Start** | The delay caused by loading a model into memory when a serverless function or container starts from idle. |
| **Model Server** | Software (e.g., Triton, TorchServe) that hosts and manages model inference at scale. |
| **Canary Deployment** | Rolling out a new model version to a small percentage of traffic first to validate before full rollout. |
| **Blue-Green Deployment** | Running two identical production environments and switching traffic from old (blue) to new (green) atomically. |
| **A/B Testing** | Routing traffic to two model variants simultaneously to compare performance metrics in production. |

---

## LLM Infrastructure

| Term | Definition |
|------|------------|
| **LLM** | Large Language Model — a neural network trained on massive text corpora capable of understanding and generating language. |
| **Foundation Model** | A large model pretrained on broad data that can be adapted to many downstream tasks. |
| **Transformer** | The neural network architecture based on self-attention that underpins most modern LLMs. |
| **Attention Mechanism** | A component that lets a model weigh the relevance of all input tokens when producing each output token. |
| **Token** | The basic unit of text (word, subword, or character) that an LLM processes. |
| **Tokenization** | The process of converting raw text into a sequence of tokens before feeding it to a model. |
| **Context Window** | The maximum number of tokens an LLM can process at once in a single input-output interaction. |
| **Prompt Engineering** | Crafting input text to guide an LLM toward desired outputs without changing its weights. |
| **System Prompt** | An initial instruction given to an LLM that sets its behavior, role, or constraints for a session. |
| **Embedding** | A dense numerical vector representation of text that captures semantic meaning. |
| **Embedding Model** | A model that converts text (or other data) into fixed-size embedding vectors. |
| **Vector** | An array of numbers representing a piece of data in a high-dimensional mathematical space. |
| **Vector Database** | A database optimized for storing and querying high-dimensional embedding vectors by similarity. |
| **Semantic Search** | Finding results based on meaning and context rather than exact keyword matching. |
| **Similarity Search** | Retrieving vectors closest to a query vector using a distance or similarity metric. |
| **ANN (Approximate Nearest Neighbor)** | An algorithm that finds near-closest vectors efficiently, trading perfect accuracy for speed at scale. |
| **HNSW** | Hierarchical Navigable Small World — a graph-based ANN algorithm widely used in vector databases. |
| **FAISS** | Facebook AI Similarity Search — a library for efficient ANN search over dense vectors. |
| **RAG (Retrieval Augmented Generation)** | Enhancing LLM responses by retrieving relevant documents at query time and injecting them into the prompt. |
| **Chunking** | Splitting large documents into smaller segments before embedding for retrieval purposes. |
| **Reranking** | A second-pass scoring step that reorders retrieved candidates by relevance before passing them to the LLM. |
| **Context Injection** | Inserting retrieved or external information into the prompt to ground the model's response. |
| **Prompt Caching** | Reusing the computed key-value state of a repeated prompt prefix to reduce latency and cost. |
| **Tool Calling** | Enabling an LLM to invoke external functions or APIs and incorporate the results into its response. |
| **Function Calling** | A structured form of tool use where the model outputs a JSON call to a predefined function. |
| **MCP (Model Context Protocol)** | An open standard for connecting LLMs to external tools, data sources, and services in a uniform way. |

---

## LLM Optimization

| Term | Definition |
|------|------------|
| **Quantization** | Reducing model weight precision (e.g., from 32-bit to 4-bit) to shrink size and speed up inference. |
| **Pruning** | Removing low-importance weights or neurons from a model to reduce its size and compute requirements. |
| **Distillation** | Training a smaller "student" model to mimic the outputs of a larger "teacher" model. |
| **LoRA** | Low-Rank Adaptation — a fine-tuning method that trains small adapter matrices instead of the full model weights. |
| **QLoRA** | Quantized LoRA — combines 4-bit quantization with LoRA adapters to fine-tune large models on consumer GPUs. |
| **PEFT** | Parameter-Efficient Fine-Tuning — a family of techniques (including LoRA) that fine-tune a small fraction of parameters. |
| **Speculative Decoding** | Using a small draft model to generate candidate tokens that the large model verifies in parallel, boosting throughput. |
| **KV Cache** | Storing previously computed key-value pairs from the attention mechanism to avoid redundant computation during generation. |
| **Prefix Caching** | Reusing the KV cache of a shared prompt prefix across multiple requests to reduce latency and cost. |
| **Flash Attention** | A memory-efficient, IO-aware exact attention algorithm that dramatically speeds up Transformer training and inference. |
| **Tensor Parallelism** | Splitting individual weight matrices across multiple GPUs to enable inference of models too large for one device. |

---

## AI Agents

| Term | Definition |
|------|------------|
| **Agent** | An LLM-powered system that autonomously perceives its environment, reasons, and takes actions to accomplish goals. |
| **Agentic Workflow** | A structured process where an LLM iterates through planning, tool use, and reflection to complete a task. |
| **Multi-Agent System** | A system where multiple specialized agents collaborate, delegate, or compete to solve complex problems. |
| **Agent Orchestration** | The coordination of multiple agents, managing task routing, communication, and execution order. |
| **Planning** | An agent's ability to decompose a high-level goal into a sequence of actionable steps. |
| **Reflection** | An agent's ability to evaluate its own outputs and decisions to correct mistakes or improve quality. |
| **Memory** | An agent's ability to store and retrieve information from past interactions or observations. |
| **Long-Term Memory** | Persistent storage of information across sessions, typically in a vector database or external store. |
| **Short-Term Memory** | In-context information available to the agent only within the current session or context window. |
| **Tool Registry** | A catalog of available tools and their schemas that an agent can consult to decide what to call. |
| **Tool Use** | An agent's ability to invoke external tools, APIs, or functions to extend its capabilities. |
| **Agent Loop** | The recurring cycle of observe → think → act that drives an agent's autonomous execution. |
| **Workflow Engine** | A system that executes and manages the steps, branching, and state of an agentic workflow. |
| **Human-in-the-Loop** | A design pattern where a human reviews, approves, or corrects agent actions at critical decision points. |

---

## Vector Databases & Search

| Term | Definition |
|------|------------|
| **Dense Embeddings** | Fixed-size vectors where all dimensions carry information, produced by neural embedding models. |
| **Sparse Embeddings** | High-dimensional vectors where most values are zero, often derived from keyword-based representations like BM25. |
| **Hybrid Search** | Combining dense (semantic) and sparse (keyword) retrieval to improve search quality. |
| **Metadata Filtering** | Narrowing a vector search to only documents matching specific attribute conditions (e.g., date, category). |
| **Retrieval** | The process of fetching the most relevant documents or chunks given a query. |
| **Indexing** | Pre-processing and organizing vectors in a data structure to enable fast similarity search at query time. |
| **ANN Index** | A data structure (e.g., HNSW, IVF) that supports fast approximate nearest neighbor lookups. |
| **Vector Similarity** | A measure of how closely related two vectors are in high-dimensional space. |
| **Cosine Similarity** | A similarity metric measuring the angle between two vectors, ignoring their magnitudes. |
| **Dot Product** | A similarity measure that multiplies corresponding vector components and sums them; effective for normalized vectors. |
| **Euclidean Distance** | A similarity metric measuring the straight-line distance between two vectors in space. |

---

## Monitoring & Observability

| Term | Definition |
|------|------------|
| **Monitoring** | Continuously tracking system health and performance metrics to detect and respond to issues. |
| **Logging** | Recording structured or unstructured events from a system for debugging and audit purposes. |
| **Tracing** | Tracking a single request as it flows across multiple services to identify latency and failures. |
| **Metrics** | Quantitative measurements of system behavior collected over time (e.g., CPU usage, error rate). |
| **Observability** | A system property that allows understanding its internal state from its external outputs (logs, metrics, traces). |
| **Model Drift** | Degradation in model performance over time as the relationship between inputs and outputs changes. |
| **Data Drift** | A shift in the statistical distribution of incoming data compared to the training data distribution. |
| **Concept Drift** | A change in the underlying real-world relationship that the model was trained to predict. |
| **Hallucination** | When an LLM generates plausible-sounding but factually incorrect or fabricated information. |
| **Evaluation** | Systematically measuring a model's quality, accuracy, or safety against defined criteria. |
| **Alerting** | Automatically notifying teams when a monitored metric crosses a defined threshold. |
| **SLA** | Service Level Agreement — a contractual commitment on system performance, availability, or uptime. |
| **SLO** | Service Level Objective — an internal target for a specific reliability or performance metric. |
| **SLI** | Service Level Indicator — the actual measured metric used to evaluate whether an SLO is being met. |

---

## Security & Governance

| Term | Definition |
|------|------------|
| **Authentication** | Verifying the identity of a user or system attempting to access a resource. |
| **Authorization** | Determining what actions an authenticated user or system is permitted to perform. |
| **RBAC** | Role-Based Access Control — granting permissions based on predefined roles assigned to users. |
| **Secrets Management** | Securely storing, rotating, and auditing access to sensitive credentials like API keys and passwords. |
| **Encryption** | Encoding data so it can only be read by parties with the correct decryption key. |
| **Compliance** | Adhering to legal, regulatory, or industry standards governing how data and systems must be managed. |
| **Audit Logging** | Recording every access and action in a tamper-resistant log for security review and compliance. |
| **Data Privacy** | Ensuring personal data is collected, stored, and used in accordance with user rights and regulations. |
| **PII** | Personally Identifiable Information — any data that can identify a specific individual (e.g., name, email). |
| **Model Governance** | Policies and processes ensuring AI models are developed, deployed, and monitored responsibly. |

---

## Popular AI Infra Tools

| Tool | Definition |
|------|------------|
| **Apache Airflow** | An open-source workflow orchestration platform for authoring, scheduling, and monitoring data pipelines as DAGs. |
| **Dagster** | A data orchestration platform focused on asset-based pipelines with built-in observability and testing. |
| **Kubeflow** | A Kubernetes-native ML platform for building, training, and deploying ML workflows at scale. |
| **MLflow** | An open-source platform for experiment tracking, model registry, and ML project reproducibility. |
| **Weights & Biases** | A cloud platform for ML experiment tracking, visualization, hyperparameter sweeps, and model management. |
| **Feast** | An open-source feature store for managing and serving ML features to models in production. |
| **Prometheus** | An open-source time-series monitoring system that scrapes and stores metrics from instrumented services. |
| **Grafana** | An open-source visualization platform for building dashboards from metrics, logs, and traces. |
| **Docker** | A platform for packaging applications into portable containers that run consistently across environments. |
| **Kubernetes** | An open-source container orchestration system for deploying, scaling, and managing containerized workloads. |
| **Pinecone** | A managed vector database optimized for large-scale, low-latency similarity search. |
| **Weaviate** | An open-source vector database with built-in vectorization, hybrid search, and GraphQL API. |
| **Qdrant** | An open-source vector database written in Rust, designed for high-performance filtered similarity search. |
| **FAISS** | A library by Meta for efficient similarity search and clustering of dense vectors at scale. |
| **vLLM** | An open-source high-throughput LLM inference engine using PagedAttention for efficient KV cache memory management. |
| **TensorRT-LLM** | NVIDIA's open-source library for optimizing and accelerating LLM inference on NVIDIA GPUs. |
| **LangChain** | A framework for building LLM-powered applications with chains, agents, and retrieval components. |
| **LlamaIndex** | A data framework for building RAG pipelines and LLM applications over custom data sources. |

---
