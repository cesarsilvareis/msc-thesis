## Thesis for Computer Science and Engineering MSc 

### Leveraging Large Language Models for Enhancing Medical Education

### Problem
This study explores the application of **Large Language Models (LLMs)** in generating pedagogical content for medical education, with a focus on the complex topic of **infective endocarditis (IE)**. While models like ChatGPT show potential, concerns arise around **accuracy, reliability**, and their ability to produce **up-to-date and medically sound information**.

### Experiments
We tested **ChatGPT (basic version)**, **GPT-4(s)**  on a variety of educational tasks, including (exclusively):
- Generating **slides, MCQs, open-ended questions**, and **clinical case studies**.
- Tailoring content for different audiences, including medical students, non-medical students, and professionals.
- **Prompt engineering** was employed for model adaptation and for assessing their contribute (in terms of medical convenience).

Additionally, we tested **state-of-the-art medical LLMs** like **MedAlpaca, ClinicalCamel, and MediTron** in explaning the concept to students of advanced medical status, which indicated us the pretrained model to fine-tune error detection for mitigating and reinforcing content generation face existing persistent of mistakes in their responses.

### Findings
- **General Language**: LLMs often lacked the necessary medical terminology for higher education levels in medicine. Dispensing with some of their application, medical LLMs possess better background and technical language.
- **Inaccurate and Outdated Information**: Outdated medical guidelines and fabricated references were frequent, particularly with the basic ChatGPT version and the custom GPT (Consensus).
- **Error Persistence**: Significant errors were found across tasks, from incorrect MCQ answers to misleading clinical case studies.
- **Limited Improvements in GPT-4**: While GPT-4 improved slightly in technical language, issues like **fraudulent references** and **inflexible content updates** remained.
- **Medical LLMs Performance**: Open-source models like **MediTron** outperformed general LLMs in **technical accuracy** and **error detection**. However, they still fell short in generating reliable educational content across all contexts, highlighting the need for more flexible fine-tuning techniques (i.e., not only relying on data and hyperparameters) and pipeline development (LangChain).

### Conclusion
While LLMs offer potential for enhancing medical education, they must be used with **expert supervision** due to persistent risks of misinformation and errors.**Always consider every LLM-generated response as your first draft**. Open-source medical LLMs show also promise but not yet fully reliable for educational purposes given their limited evaluation -> reliance on benchmarks of knowledge, and application -> fine/instruction-tuning need high-quality medical data (which is scarce...).

### Available Access
All project work is restricted by the authors' considerations and declarations. Part of such is publicaly provided in this repository:

- Dissertation: [extended abstract document](extended_abstract.pdf);  
- Implementation code: [application and access conditions](https://github.com/cesarsilvareis/llm-manager/tree/master);
- Results: [reported evidences](prompting/).

