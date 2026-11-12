# Titanic survival dashboard

Interactive Streamlit view of the 891-passenger Titanic dataset in `data/titanic.csv`.

A 3D scene in `scene/index.html` (three.js, loaded from a CDN) shows the ship hitting the iceberg, lifeboats being lowered, and passengers jumping into the sea and drowning. Each figure stands for about 15 passengers. Clothing colour is the class, a dress is a woman and a suit is a man. The scene is a two-way Streamlit component: clicking a lifeboat filters to survivors, and clicking a person or a lifebelt filters to their sex, class and outcome. Clicking the same thing again shows everyone.

The page uses a navy-and-gold ship theme. The sidebar filters sex, outcome, travel party, cabin record, class, embarkation port, age, and fare. Cards and charts follow that selection and compare the survival rate with the full ship.

Photos in `assets/` are public-domain images of the ship leaving Southampton and Willy Stöwer's 1912 painting.

Needs `streamlit`, `pandas`, and `altair` (`altair` is installed with Streamlit).

```bash
python -m streamlit run titanic_dashboard.py
```

Streamlit prints the local URL when it starts. The default port is 8501.
