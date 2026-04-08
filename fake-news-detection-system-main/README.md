📰 Fake News Detection System

A multi-stage Fake News Detection System that evaluates the authenticity of news articles using a structured compartment-based analysis approach. The system processes user-submitted content and provides a final verdict based on reliability, legitimacy, and trustworthiness.

🚀 Features
🔍 Stage 1: Quick Authenticity Filter
Checks source credibility
Evaluates content quality
Filters spam or low-quality inputs
⚙️ Stage 2: Preprocessing & Data Extraction
Extracts text, metadata, keywords
Prepares content for deeper analysis
📊 Compartment-Based Analysis
C1 – Relatability
Checks contextual relevance (location, time, plausibility)
C2 – Legitimacy
Compares with trusted sources
Measures similarity and cross-references
C3 – Trustworthiness
Evaluates bias, factual consistency, and source reliability
🧮 Score Calculation

Weighted scoring system:

Final Score = 
0.55 × Legitimacy +
0.30 × Relatability +
0.15 × Trustworthiness
🏁 Final Verdict
VERIFIED
SUSPICIOUS
NEEDS REVIEW
FAKE
🧩 System Workflow
User
↓
Stage 1: Input Collection
↓
Stage 2: Preprocessing
↓
Compartment 1 → Compartment 2 → Compartment 3
↓
Calculate Scores
↓
Display Results
🛠️ Tech Stack
Frontend: React + TypeScript
Backend: Supabase (Edge Functions)
APIs: News data integration (trusted sources)
Processing: Custom scoring algorithms
📂 Project Structure
├── src/
│   ├── components/
│   ├── services/
│   │   ├── stage1Service.ts
│   │   ├── newsAnalysisService.ts
│   ├── pages/
│   └── utils/
│
├── supabase/
│   ├── functions/
│   │   ├── stage1-filter/
│   │   ├── verify-news/
│
└── README.md
⚙️ How It Works
User submits news content (text or URL)
Stage 1 filters low-quality or suspicious input
Stage 2 processes and extracts key information
Content is analyzed across three compartments
Scores are calculated using weighted formulas
Final verdict is generated and displayed
📊 Example Output
{
  "relatabilityScore": 65,
  "legitimacyScore": 78,
  "trustworthinessScore": 40,
  "finalScore": 68,
  "verdict": "SUSPICIOUS"
}
🎯 Objectives
Detect misleading or false information
Provide explainable scoring instead of black-box results
Improve reliability of news consumption
Support users in critical evaluation of content
🔮 Future Improvements
Real-time fact-checking integration
Advanced NLP-based contextual analysis
User feedback learning system
Dashboard for analytics and trends
🤝 Contributing

Contributions are welcome!
Feel free to fork the repo and submit a pull request.

📜 License

This project is licensed under the MIT License.

👨‍💻 Author

Developed as part of a project on Fake News Detection using Multi-Stage Analysis System
