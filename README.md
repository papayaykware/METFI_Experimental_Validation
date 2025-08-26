# METFI_Experimental_Validation
Validación experimental del Modelo Electromagnético Toroidal de Forzamiento Interno (METFI) del Sistema Tierra. Incluye protocolos de infraestructura, diseño de instrumentación, métodos de registro y esquemas para diferenciar señales METFI de ruido ambiental. Integra datasets abiertos de magnetometría, ionosfera y bioelectromagnetismo
# METFI: Validación Experimental y Metodológica

## Resumen
Este repositorio documenta los procedimientos, protocolos y metodologías orientadas a la validación experimental del Modelo Electromagnético Toroidal de Forzamiento Interno (METFI) del Sistema Tierra. Se centra en:

- Diseño de infraestructura instrumental.
- Métodos de registro de señales electromagnéticas.
- Protocolos de filtrado y análisis para diferenciar señales METFI de ruido ambiental.
- Integración de datasets abiertos de magnetometría, ionosfera y bioelectromagnetismo.

El objetivo es establecer un marco reproducible para estudios observacionales y simulaciones experimentales de fenómenos toroidales internos.

## Estructura del Repositorio

METFI_Experimental_Validation/
│
├── docs/ # Documentación de protocolos e instrumentación
├── datasets/ # Conexiones a datasets abiertos
├── scripts/ # Scripts de procesamiento de señales y análisis
├── diagrams/ # Diagramas de instrumentación y flujos de datos
├── README.md
└── LICENSE


## Protocolos de Instrumentación

### Sensores recomendados:
- Magnetómetros triaxiales de alta sensibilidad (0.1 nT resolución).
- Antenas de bobina de inducción para medición de campos de baja frecuencia.
- Sensores de plasma y ionosfera (redes GNSS, ionosondes).
- Bioelectromagnetismo: electrodos EEG/EMG adaptados a registro ambiental.

### Infraestructura:
- Estaciones de registro distribuidas para cobertura global.
- Acondicionamiento electromagnético: blindaje parcial, reducción de ruido urbano.
- Sincronización temporal por GPS para correlación de señales.

### Métodos de registro:
- Muestreo continuo y por ráfaga.
- Almacenamiento en formatos abiertos (.csv, HDF5).
- Metadatos estandarizados (latitud, longitud, altitud, timestamp, sensor type).

## Esquema Comparativo: Señal METFI vs Ruido Ambiental

1. **Análisis espectral**: identificar bandas características toroidales.
2. **Correlación temporal**: verificar coherencia en estaciones múltiples.
3. **Filtrado adaptativo**: eliminar interferencias de red eléctrica, radiofrecuencia y geomagnéticas conocidas.
4. **Validación cruzada**: usar datasets históricos de magnetometría y ionosfera para descartar eventos coincidentes no METFI.

## Datasets Abiertos Sugeridos

- [INTERMAGNET](https://www.intermagnet.org/) – Datos globales de magnetometría.
- [NASA CDAWeb](https://cdaweb.gsfc.nasa.gov/) – Plasma y campos electromagnéticos en ionosfera.
- [OpenNeuro](https://openneuro.org/) – Bioelectromagnetismo para análisis comparativo de ruido ambiental.

## Scripts y Ejemplos

- `scripts/signal_processing.py`: filtrado de ruido y extracción de características toroidales.
- `scripts/cross_validation.ipynb`: correlación multiestación y comparación con datasets históricos.
- `diagrams/instrument_layout.png`: disposición recomendada de sensores y antenas.

## Licencia
Este proyecto se distribuye bajo la **Licencia MIT**.

## Contribuciones
Se aceptan contribuciones relacionadas con:
- Nuevos protocolos de instrumentación.
- Métodos avanzados de filtrado de señal.
- Integración de datasets adicionales de magnetometría, ionosfera o bioelectromagnetismo.
