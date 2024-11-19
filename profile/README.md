# 🎓 Distribution of Courses Without Envy

**A project focused on implementing innovative algorithms for fair and envy-free course allocation.** This work combines advanced theoretical concepts with practical applications, culminating in robust algorithms and an interactive demonstration website.

---

## 📚 Problem Statement  
Universities face significant challenges in allocating limited courses among students with diverse preferences while ensuring fairness. Traditional methods often fall short, resulting in envy or inefficiencies. Our project tackles this problem by developing novel algorithms based on the *Approximate Competitive Equilibrium from Equal Incomes (A-CEEI)* framework, ensuring:  
- **⚖️ Fairness**: Students receive allocations proportional to their budgets and preferences.  
- **🤝 Envy Minimization**: Reducing the likelihood of students envying others’ allocations.  
- **🚀 Efficiency**: Balancing computational performance with allocation quality.  

---

## 🛠️ Our Contributions  

### 1. Algorithm Development  
We implemented three advanced algorithms, integrated into the `fairpyx` library:  
- **🧮 ACEEI**:  
  - Finds market-clearing prices and optimal allocations under Envy-Free-but-for-Tie-Breaking (EF-TB) constraints.  
  - Balances supply and demand efficiently using parameters like budget perturbations (`epsilon`) and price adjustments (`delta`).  
- **🔍 Find Manipulation**:  
  - Identifies and evaluates possible strategic manipulations.  
  - Ensures robustness against student misreporting of preferences.  
- **♟️ Tabu Search**:  
  - Utilizes heuristic optimization to explore neighborhoods of price vectors.  
  - Incorporates history, caching, and threading for improved performance.  

> **📂 Location**: [ACEEI_algorithms folder](https://github.com/Final-project-distribution-of-courses/Distribution_of_courses/tree/main/fairpyx/algorithms/ACEEI_algorithms).  

---

### 2. ⚗️ Experimentation and Benchmarking  
We conducted extensive experiments to evaluate:  
- **⚡ Performance**:  
  - Compared runtimes of our algorithms against existing methods in the `fairpyx` library, such as `iterated maximum matching` and `bidirectional round robin`.  
  - Demonstrated significant improvements through optimizations like threading and caching.  
- **🧑‍🤝‍🧑 Fairness Metrics**:  
  - Measured Utilitarian Social Welfare (USW) and Nash Social Welfare (NSW).  
  - Showed superior fairness outcomes, especially under contested EF-TB constraints.  
- **🔒 Manipulation Resistance**:  
  - Validated the robustness of our algorithms against strategic misreports in diverse scenarios.  

---

### 3. 🌐 Interactive Demonstration Website  
We built a Flask-based website to showcase our algorithms in action:  
- **✨ Features**:  
  - Run experiments with custom or random parameters (e.g., number of students, courses, budgets).  
  - View detailed results and allocation outputs.  
- **🎨 User-Friendly Design**:  
  - Explains each algorithm with step-by-step visualizations.  
  - Encourages engagement with practical examples.  

> **🔗 Website Link**: [Interactive Website](https://renanaturgeman058.csariel.xyz/)  
> **📂 Website Repository**: [Flask-Website](https://github.com/Final-project-distribution-of-courses/Flask-Website).  

---

## 🏗️ Technical Challenges and Solutions  
- **📊 Efficient Market-Clearing**: Achieved zero market-clearing error by balancing step size (`delta`) and budget perturbation (`epsilon`).  
- **⚙️ Scalability**: Optimized Tabu Search using threading, caching, and C++ integration for runtime improvements.  
- **⚖️ Fairness vs. Performance Trade-Off**: Balanced these competing objectives to ensure practical application.  

---

## 🌟 Impact and Outcome  
- **💡 Innovation**:  
  - Improved fairness mechanisms over traditional algorithms.  
  - Established benchmarks for envy-free and efficient allocations.  
- **🏫 Practical Application**:  
  - Demonstrated usability in course allocation systems through an interactive website.  
  - Created a robust and reusable extension to the `fairpyx` library.  

---

## 📁 Repositories  
1. **💻 Core Implementation**:  
   [Distribution_of_course](https://github.com/Final-project-distribution-of-courses/Distribution_of_courses)  
   - Location of the algorithms ([ACEEI_algorithms folder](https://github.com/Final-project-distribution-of-courses/Distribution_of_courses/tree/main/fairpyx/algorithms/ACEEI_algorithms)).  
   - Scripts for experimentation and performance evaluation.  

2. **🌐 Website Demonstration**:  
   [Flask-Website](https://github.com/Final-project-distribution-of-courses/Flask-Website)  
   - Source code for the interactive demonstration website.  

---

## 🤝 Acknowledgments  
This project would not have been possible without the guidance and support of **[Erel Segal-Halevi](https://github.com/erelsgl)**, the author of the `fairpyx` library. His insights and expertise were invaluable in shaping the algorithms and ensuring the project's success.  

We also thank the authors of the *A-CEEI* article for their foundational work on which this project builds.  

---

## 👩‍💻 About Us  
This project was collaboratively developed by:  
- **[Renana Turgeman](https://github.com/RenanaTurgeman)**
- **[Erga Bar-Ilan](https://github.com/ErgaDN)**
- **[Ofir Shitrit](https://github.com/ofirshitrit)** 

---

## 📬 Get in Touch  
For inquiries or collaboration opportunities, feel free to:  
- Open an issue in one of the repositories.  
- Visit our demonstration website: [Interactive Website](https://renanaturgeman058.csariel.xyz/).  

---
