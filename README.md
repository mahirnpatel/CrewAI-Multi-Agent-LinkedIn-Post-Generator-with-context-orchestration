# LinkedIn Post Generator using CrewAI

A structured multi-agent LinkedIn post generator built using CrewAI to demonstrate context passing, API integration, and orchestration in AI systems.

---

## Project Objective

This project was built to deeply understand how structured multi-agent workflows operate inside CrewAI.

Instead of simply generating content, the goal was to explore:

- Context passing between agents  
- External API integration (Serper API)  
- Task sequencing inside a Crew  
- Abstraction layers in orchestration frameworks  

The focus was on system design — not just output generation.

---

## System Architecture

The workflow consists of three specialized agents working sequentially.

### Analyst Agent – Information Gathering

- Uses the Serper API to search the web based on a given topic  
- Collects relevant information  
- Passes structured context forward  

This agent is responsible for raw data acquisition.

---

### Research Analyst Agent – Context Refinement

- Takes raw search results  
- Filters noise  
- Extracts meaningful insights  
- Structures the information  

This agent transforms raw data into usable intelligence.

---

### Writer Agent – Content Generation

- Receives structured insights  
- Generates a professional LinkedIn post  
- Ensures clarity, structure, and engagement  

This agent focuses purely on writing — not research.

---

## Workflow Orchestration

CrewAI coordinates:

1. Task sequencing  
2. Context passing between agents  
3. Controlled execution  
4. Modular collaboration  

This structured orchestration improves reliability and clarity in agentic systems.

---

## Key Concepts Demonstrated

- Multi-agent collaboration  
- Structured context propagation  
- API integration within agent pipelines  
- Separation of responsibilities  
- Workflow abstraction using frameworks  

---

## Major Takeaway

Strong AI systems are not just about generating outputs.

They rely on:

- Structured context flow  
- Controlled execution  
- Modular design  
- Clear role separation  

Frameworks like CrewAI do not replace understanding — they enhance productivity once fundamentals are clear.

---

## Tech Stack

- Python  
- CrewAI  
- Serper API  
- Large Language Model (LLM Provider)  

---

## Example Use Case

Input: Topic: System on Chip (SoC)

Output:
- Research-backed  
- Structured  
- Professional LinkedIn post  
- Ready to publish  

---

## Setup Instructions

1. Clone the repository
```bash
git clone 
cd 
```

2. Create virtual environment
```bash
python -m venv .venv
source .venv/bin/activate  
```
3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Create `.env` file
```bash
SERPER_API_KEY=your_key_here
OPENAI_API_KEY=your_key_here
```

5. Run the project
```bash
crewai run 
```
---

## Future Improvements

- Add memory layer for iterative refinement  
- Add tone customization (technical, storytelling, thought leadership)  
- Add UI layer (Streamlit or Gradio)  
- Add evaluation agent for output scoring 