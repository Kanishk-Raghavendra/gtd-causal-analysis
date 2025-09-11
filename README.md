# A Multi-Outcome Causal Analysis of Post-9/11 Airport Security

## Project Description
This project conducts a rigorous causal analysis to measure the true impact of the global airport "hardening" policies enacted after the 9/11 attacks.  
It moves beyond a simple evaluation of effectiveness to investigate the potential unintended consequences of this policy.  

The analysis uses a **Difference-in-Differences (DiD)** methodology to isolate the causal effect of the security mandates from other confounding trends and explores three distinct outcomes:
- **Policy Effectiveness**
- **Displacement of Attacks**
- **Tactical Adaptation of Terrorists**

---

## Key Research Questions
1. **Effectiveness**: Did the security mandates causally reduce the frequency of attacks against airports and aircraft?  
2. **Displacement**: Did hardening airports lead to a "spillover" effect, causing an increase in attacks on alternative, "softer" transportation targets?  
3. **Tactical Adaptation**: Did the policies force terrorists to change their methods, potentially affecting the lethality or weapon sophistication of subsequent attacks?  

---

## Dataset
- **Source**: Global Terrorism Database (GTD)  
- **Size**: 180,000+ terrorist attacks worldwide (1970–2017)  
- **Provider**: National Consortium for the Study of Terrorism and Responses to Terrorism (START)  
- **Access**: [Kaggle – Global Terrorism Database](https://www.kaggle.com/START-UMD/gtd)  

---

## Methodology
The core of this project is a **Difference-in-Differences (DiD)** causal inference model.  
This quasi-experimental method estimates the effect of an intervention by comparing outcome changes over time between a treatment group and a control group.

- **Intervention**: Implementation of global, intensive airport security protocols post-9/11.  
- **Treatment Group**: Attacks targeting *Airports & Aircraft*.  
- **Control Group**: Attacks targeting other *Transportation* infrastructure (e.g., buses, trains, subways).  
- **Key Assumption**: The **Parallel Trends Assumption**—that both groups followed a similar trend in attack frequency before the intervention.  

---

## Project Structure
```bash
gtd-causal-analysis/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── reports/
├── figures/
└── src/
```
## Setup and Installation
```bash
#Clone the repository
git clone https://github.com/your-username/gtd-causal-analysis.git
cd gtd-causal-analysis

#Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

#Install dependencies
pip install -r requirements.txt
```
