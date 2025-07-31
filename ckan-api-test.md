---
jupytext:
  formats: ipynb,md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: '0.13'
    jupytext_version: 1.14.0
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---


# 實際透過 API 測試查詢 depositar 資料集 API
> demo server 不需要 API token

depositor demo site, project [url](https://demo.depositar.io/zh_Hant_TW/organization/penghu-soundscape-sample-dataset)
## 查詢 metadata

```{code-cell} ipython3
import requests
import json

dataset_id = "0ae75957-f2da-4e0e-bbb1-cdddc8345f00"
url = f"https://demo.depositar.io/api/3/action/package_show?id={dataset_id}"

res = requests.get(url)
data = res.json()

# 顯示資料集中的資源清單
resources = data["result"]["resources"]
for r in resources:
    print(f"Result: ")
    print(f"- {r['name']} ({r['format']}) → {r['url']}")
```

---

## Dataset Title

```{code-cell} ipython3
print(f"Result: ")
print("Dataset title:", data["result"]["title"])
```
