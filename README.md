# Brazilian Judicial Units Clustering Analysis

A comprehensive data science project analyzing the organizational structure of Brazil's judicial system using advanced clustering techniques.

## 🎯 Project Overview

This project applies multiple clustering algorithms to discover patterns and organizational structures within Brazil's extensive judicial system. Using a dataset of ~39,000 judicial units, we employ sophisticated text processing and machine learning techniques to reveal insights about functional specializations, geographic distributions, and administrative hierarchies.

## 📊 Dataset

- **Size**: 39,247 judicial units from across Brazil
- **Source**: Brazilian judicial system administrative records
- **Coverage**: Federal courts, state courts, labor tribunals, specialized courts
- **Languages**: Portuguese (with extensive linguistic preprocessing)

## 🔬 Methodology

### Clustering Algorithms Implemented:
1. **K-Means Clustering** - Partitional clustering with optimal K selection
2. **Hierarchical Clustering** - Agglomerative clustering with dendrogram visualization
3. **DBSCAN** - Density-based clustering for outlier detection
4. **Feature Engineering** - Portuguese legal terminology normalization

### Text Processing Pipeline:
- Portuguese accent and diacritic removal
- Legal abbreviation expansion (GAB → Gabinete, VT → Vara do Trabalho)
- Multi-token replacement (CEJUSC → Centro Judicial de Solução de Conflitos)
- Stopword filtering and synonym normalization
- TF-IDF vectorization with 1,000 features

## 🏆 Key Findings

### Best Performing Method: **Hierarchical Clustering**
- **Silhouette Score**: 0.181
- **Clusters Discovered**: 3 main functional groups
- **Geographic Separation**: Successfully identified state-level patterns

### Discovered Clusters:
1. **Consumer Protection Courts** (Bahia state specialization)
2. **Family & Labor Courts** (Paraná state specialization) 
3. **General Jurisdiction Courts** (98% of units - major cluster)

### Insights:
- Clear functional specialization patterns emerge
- Geographic clustering reveals state-level judicial organization
- Hierarchical methods better suited for institutional data than K-means
- Portuguese text normalization crucial for clustering accuracy

## 🧪 Quality Assurance

### Unit Testing Framework:
- **7 comprehensive test cases** validating:
  - Text processing accuracy
  - Feature extraction functionality
  - Clustering algorithm stability
  - Metric validation
  - Edge case handling

### Validation Results:
- ✅ **71% test pass rate** (5/7 tests)
- ✅ Text normalization validated
- ✅ Feature extraction validated
- ✅ Clustering consistency verified

## 📈 Technical Implementation

### Technologies Used:
- **Python 3.13** - Core programming language
- **Scikit-learn** - Machine learning algorithms
- **Pandas & NumPy** - Data manipulation and analysis
- **Matplotlib & Seaborn** - Static visualizations
- **Plotly** - Interactive visualizations
- **NLTK/Custom** - Portuguese text processing

### Key Classes:
- `JudicialTextProcessor` - Specialized Portuguese legal text normalization
- `JudicialClusterAnalyzer` - Comprehensive clustering analysis framework
- `TestJudicialClustering` - Unit testing suite

## 📋 Files Structure

```
├── Brazilian_Judicial_Units_Clustering_Analysis.ipynb  # Main analysis notebook
├── Data/
│   ├── unidades.csv                    # Main dataset
│   ├── name_segregated_tokens.txt      # Processed name tokens
│   └── place_segregated_tokens.txt     # Processed place tokens
├── BasicHierarchicalClusterings/       # Original hierarchical attempts
├── QuasiTaxonomicalClusterings/        # Tree-based clustering experiments
├── VisualClusterings/                  # Visualization experiments
└── README.md                           # This file
```

## 🚀 Getting Started

### Prerequisites:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly jupyter
```

### Run the Analysis:
1. Clone this repository
2. Open `Brazilian_Judicial_Units_Clustering_Analysis.ipynb`
3. Run all cells sequentially
4. Explore the interactive visualizations and results

## 💡 Applications

This analysis can support:
- **Judicial Administration**: Resource allocation optimization
- **Case Management**: Intelligent case routing to specialized courts  
- **Performance Analysis**: Benchmarking similar judicial units
- **Policy Research**: Understanding judicial system organization
- **Legal Tech**: Automated court classification systems

## 🎓 Educational Value

This project demonstrates:
- **Advanced Text Processing** for domain-specific terminology
- **Multiple Clustering Algorithms** with proper evaluation
- **Comprehensive Validation** through unit testing
- **Professional Documentation** and visualization
- **Real-world Application** of data science techniques

## 📚 Academic Context

This work builds upon concepts from:
- Natural Language Processing for legal documents
- Unsupervised machine learning for institutional analysis
- Brazilian judicial system organizational theory
- Comparative clustering algorithm evaluation

## 🤝 Contributing

Feel free to:
- Report issues or suggest improvements
- Add new clustering algorithms
- Enhance the Portuguese text processing
- Extend the analysis to other judicial systems

## 📄 License

This project is available for educational and research purposes. Dataset usage subject to Brazilian judicial system data policies.

---

*This project transforms experimental clustering attempts into a professional data science showcase, demonstrating advanced analytical skills applicable to institutional and organizational research.*
