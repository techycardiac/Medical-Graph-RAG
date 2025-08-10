# AI Assistant Examples for Medical-Graph-RAG

This document provides specific examples of how to use AI assistants effectively with this Medical-Graph-RAG repository.

## 🏥 Repository-Specific Use Cases

### Medical Data Processing
```markdown
**Good Request**: "Optimize the medical text chunking in data_chunk.py to handle larger documents more efficiently"
**Context**: The current chunking process is slow for large medical textbooks
**Expected Outcome**: Faster processing with maintained accuracy
```

### Graph Construction
```markdown
**Good Request**: "Add error handling to the Neo4j graph creation in creat_graph.py for connection failures"
**Context**: Users experience crashes when Neo4j is unavailable
**Expected Outcome**: Graceful handling with informative error messages
```

### RAG System Enhancement
```markdown
**Good Request**: "Implement caching for the retrieval system to avoid duplicate medical paper queries"
**Context**: Current system re-processes the same queries repeatedly
**Expected Outcome**: 50% reduction in query processing time
```

## 🔧 Common Maintenance Tasks

### Environment & Dependencies
- **Conda Environment Issues**: "Fix dependency conflicts in medgraphrag.yml for Python 3.11 compatibility"
- **Docker Improvements**: "Update Dockerfile to use multi-stage builds for smaller image size"
- **Package Updates**: "Update CAMEL framework to latest version and fix any breaking changes"

### Code Quality
- **Error Handling**: "Add comprehensive error handling to the UMLS data processing pipeline"
- **Logging**: "Implement structured logging throughout the graph construction process"
- **Type Hints**: "Add type annotations to improve code clarity and IDE support"

### Testing
- **Unit Tests**: "Create unit tests for the agentic_chunker.py functions"
- **Integration Tests**: "Add tests for the complete RAG pipeline with mock data"
- **Performance Tests**: "Create benchmarks for graph query response times"

## 📊 Performance Optimization Examples

### Database Optimization
```markdown
**Request**: "Optimize the Neo4j queries in retrieve.py for faster medical concept retrieval"
**Background**: Current queries take 5+ seconds for complex medical relationships
**Goal**: Reduce query time to under 2 seconds while maintaining accuracy
```

### Memory Usage
```markdown
**Request**: "Reduce memory consumption in the graph construction process for large medical datasets"
**Context**: Current process uses 16GB+ RAM for medium-sized medical corpora
**Requirement**: Process same data with under 8GB RAM usage
```

## 🔒 Security & Compliance

### Data Privacy
```markdown
**Request**: "Implement data anonymization for patient records before graph processing"
**Compliance**: Must follow HIPAA guidelines for medical data handling
**Requirement**: Remove all PII while preserving medical relationships
```

### API Security
```markdown
**Request**: "Add API key validation and rate limiting to the RAG query endpoint"
**Context**: Current demo allows unlimited queries without authentication
**Goal**: Secure production deployment with proper access controls
```

## 📚 Documentation Improvements

### User Guides
- **Setup Instructions**: "Create step-by-step setup guide for Windows users"
- **API Documentation**: "Document all available parameters for the GraphRAG class"
- **Troubleshooting**: "Add FAQ section for common Neo4j connection issues"

### Developer Documentation
- **Architecture Diagrams**: "Create visual documentation of the multi-agent pipeline"
- **Code Comments**: "Add detailed docstrings to all utility functions in utils.py"
- **Contributing Guide**: "Create guidelines for external contributors"

## 🚀 Feature Development Examples

### New Capabilities
```markdown
**Request**: "Add support for medical image analysis in the RAG pipeline"
**Requirements**: 
- Integrate with medical imaging APIs
- Extract relevant metadata for graph construction
- Maintain DICOM compliance
```

### User Interface
```markdown
**Request**: "Create a web interface for the medical graph query system"
**Features Needed**:
- Medical professional authentication
- Interactive graph visualization
- Query history and bookmarking
```

### Data Sources
```markdown
**Request**: "Add integration with PubMed Central API for real-time medical literature"
**Requirements**:
- Respect API rate limits
- Cache frequently accessed papers
- Update graph with new publications automatically
```

## ⚠️ Repository-Specific Considerations

### Medical Domain Constraints
- **Accuracy Critical**: All changes must maintain medical accuracy
- **Compliance Requirements**: Consider HIPAA, FDA, and other medical regulations
- **Validation Needed**: Medical professionals should validate domain-specific changes

### Technical Constraints
- **Large Data Handling**: Medical datasets are typically very large
- **Graph Complexity**: Medical relationships create complex graph structures
- **Real-time Requirements**: Clinical applications need fast response times

### Dependencies
- **CAMEL Framework**: Changes must be compatible with multi-agent architecture
- **Neo4j**: Graph operations must follow best practices for medical data
- **UMLS Integration**: Maintain compatibility with medical terminology standards

## 📋 Request Templates for This Repository

### Bug Fix Template
```markdown
**Issue**: [Specific medical RAG functionality that's broken]
**Error Details**: [Stack trace or error message]
**Medical Context**: [What medical use case is affected]
**Test Data**: [Sample medical data that reproduces the issue]
**Expected Medical Outcome**: [What should happen from medical perspective]
```

### Feature Request Template
```markdown
**Medical Use Case**: [Specific clinical or research scenario]
**Current Limitation**: [What doesn't work currently]
**Proposed Solution**: [How this would help medical professionals]
**Data Requirements**: [What medical data sources needed]
**Validation Criteria**: [How to verify medical accuracy]
```

### Performance Optimization Template
```markdown
**Current Performance**: [Specific metrics: query time, memory usage, etc.]
**Medical Context**: [Clinical scenario requiring better performance]
**Target Performance**: [Specific improvement goals]
**Constraints**: [Medical accuracy, compliance requirements]
**Test Dataset**: [Representative medical data for benchmarking]
```

---

*These examples help you work effectively with AI assistants on medical AI projects while maintaining the high standards required for healthcare applications.*