# N3uron_I3X
This project is a high-performance FastAPI-based implementation of the I3X (Industrial Information Interface eXchange) API as defined in RFC 001. It serves as a Contextualized Manufacturing Information Platform (CMIP) that allows for browsing, querying, and subscribing to industrial data in a standardized format.
🚀 Key Features
Standardized API: Implements RFC 001 compliant endpoints for Namespaces, Object Types, Relationships, and Instance management.
Unified Data Access: Aggregates data from multiple industrial sources into a single, contextualized model.
Real-time Subscriptions: Supports live data streaming of sensor and machine values using the I3X subscription model.
Multi-Source Routing: Advanced configuration that routes specific operations (e.g., metadata browsing vs. real-time values) to different specialized backends for optimal performance.
Interactive Documentation: Built-in Swagger UI and ReDoc for easy API exploration and testing.
🔌 Supported Data Sources
The server features a modular adapter architecture, with a primary focus on the N3uron integration:

N3uron REST Adapter:
Real-time polling of N3uron groups and tags.
Dynamic mapping of N3uron hierarchical structures to I3X folders and measurements.
Automatic quality and timestamp conversion.
