# AgenteIA_LevantamientodeCargasLaborales
Agente de Inteligencia Artificial tipo ChatBot para asistir al proceso de Levantamiento de Cargas Laborales de la Gerencia de Efectividad Organizacional para el Banco de Bogotá.

flowchart TD

subgraph group_runtime["Agent Runtime"]
  node_chatbot["AI Chatbot"]
end

subgraph group_domain["Business Process"]
  node_workload["Workload Assessment"]
end

node_employee(("Employee"))
node_effectiveness(("Organizational Effectiveness"))

node_employee -->|"provides input"| node_chatbot
node_chatbot -->|"assists process"| node_workload
node_workload -->|"supports review"| node_effectiveness

click node_chatbot "https://github.com/bl8dyg1rl/agenteia_levantamientodecargaslaborales/blob/main/AgenteIA_LevantamientodeCargas_PruebaFinal.ipynb"
click node_workload "https://github.com/bl8dyg1rl/agenteia_levantamientodecargaslaborales/blob/main/AgenteIA_LevantamientodeCargas_PruebaFinal.ipynb"

classDef toneNeutral fill:#f8fafc,stroke:#334155,stroke-width:1.5px,color:#0f172a
classDef toneBlue fill:#dbeafe,stroke:#2563eb,stroke-width:1.5px,color:#172554
classDef toneAmber fill:#fef3c7,stroke:#d97706,stroke-width:1.5px,color:#78350f
classDef toneMint fill:#dcfce7,stroke:#16a34a,stroke-width:1.5px,color:#14532d
classDef toneRose fill:#ffe4e6,stroke:#e11d48,stroke-width:1.5px,color:#881337
classDef toneIndigo fill:#e0e7ff,stroke:#4f46e5,stroke-width:1.5px,color:#312e81
classDef toneTeal fill:#ccfbf1,stroke:#0f766e,stroke-width:1.5px,color:#134e4a
class node_chatbot toneBlue
class node_workload toneAmber
class node_employee,node_effectiveness toneIndigo
