# Python — Working with JSON Files

A hands-on Jupyter Notebook covering JSON file handling in Python from basics to real-world examples.

## Topics covered

| Topic | Function used |
|---|---|
| Convert dict to JSON string | `json.dumps()` |
| Convert JSON string to dict | `json.loads()` |
| Write JSON to file | `json.dump()` |
| Read JSON from file | `json.load()` |
| Pretty print JSON | `indent=4` parameter |
| Modify and update JSON file | Read → edit → write |
| Work with JSON arrays | `for` loop iteration |

## Datasets used

- `Person_detail.json` — simple person record
- `airports.json` — 20+ international airports with IATA codes, coordinates
- `Student_detail.json` — student records with ID, name, salary
- `marks.json` — student marks data

## Key concepts

- Difference between `dumps/loads` (in-memory) vs `dump/load` (file-based)
- Accessing nested JSON keys: `data["City"]`, `ai["code"]`
- Iterating over JSON arrays with `for` loops
- Saving files to specific directory paths with `os.getcwd()`

## How to run

```bash
pip install jupyter
jupyter notebook Work_with_JSON_File.ipynb
```
