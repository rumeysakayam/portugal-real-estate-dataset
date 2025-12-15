# Portugal Real Estate Dataset

Complete building dataset for Portugal extracted from OpenStreetMap for real estate intelligence and analysis.

## 📋 Attributes

Each building includes:
- Geometry (location and shape)
- Building type (residential, commercial, etc.)
- Calculated area (m²)
- Building levels (4.6% coverage)
- Height data (0.8% coverage)
- Street addresses (5.4% coverage)

## 🛠️ Methodology

1. **Data Extraction:** Downloaded Portugal OSM data from Geofabrik (.pbf format)
2. **Processing:** Extracted buildings using pyrosm library
3. **Area Calculation:** Converted to EPSG:3763 (Portugal TM06) for accurate measurements
4. **Quality Filtering:** Removed buildings <10 m² or >50,000 m² (likely errors)
5. **Validation:** 97.7% of original dataset passed quality checks

## 🚀 Usage

The processed dataset is available as `portugal_buildings_processed.geojson` (2.4 GB).

**Note:** Data files are not stored in this repository due to size constraints.

## 📝 License

Data sourced from OpenStreetMap © OpenStreetMap contributors  

**Rumeysa Kayam**  
Data Science Intern @ 5steps real estate

---

*Building the foundation for data-driven real estate investment analysis in Portugal*
