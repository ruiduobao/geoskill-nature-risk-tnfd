# geoskill-nature-risk-tnfd

> TNFD LEAP-based nature-related financial risk screening. Locates enterprise assets relative to protected areas, water stress, and forest cover; evaluates nature dependency and impact using sector materiality; produces priority risk inventory and audit-ready evidence package.

See [SKILL.md](SKILL.md) for full usage, inputs and outputs.

## Quick start

```bash
# Synthetic demo mode (no input files needed)
python scripts/nature_risk_tnfd.py --output-dir ./nrt-output

# With custom assets file (GeoJSON or CSV)
python scripts/nature_risk_tnfd.py --assets ./my-assets.geojson --output-dir ./nrt-output

# With sector override and custom buffers
python scripts/nature_risk_tnfd.py --sector agriculture --buffers "facility:5000,watershed:10000" --output-dir ./nrt-output

# With all parameters
python scripts/nature_risk_tnfd.py --assets ./assets.csv --sector mining --buffers "facility:10000" --indicators-config ./my-indicators.json --output-dir ./nrt-output
```

## License

MIT
