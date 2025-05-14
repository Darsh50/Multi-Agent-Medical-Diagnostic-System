# Multi-Agent-Medical-Diagnostic-System

<img width="900" alt="image" src="https://github.com/Darsh50/Multi-Agent-Medical-Diagnostic-System/blob/main/Assests/img.png">

A GPT-powered multi-agent framework for collaborative medical diagnosis and treatment suggestions

## Current Implementation Overview

In the current implementation, three GPT-4o-based AI agents each focused on a unique medical specialty analyze a patient report in parallel using threading. Each agent delivers a diagnosis and treatment suggestions from their area of expertise. Their individual insights are then aggregated by a summarizing model, which synthesizes the findings and highlights three likely health conditions relevant to the patient’s symptoms.

### AI Agents

**1. Cardiologist Agent**

- **Role**: Identify any potential cardiac issues that could explain the patient's symptoms, including ruling out conditions such as arrhythmias or structural abnormalities that might not be apparent in initial evaluations.
  
- **Action**: Recommends further cardiovascular diagnostics (e.g., continuous monitoring or tests) and outlines treatment options if cardiac issues are detected.

**2. Psychologist Agent**

- **Role**: Determine if the symptoms align with a psychological condition, such as panic disorder or another anxiety-related issue. Assess the impact of stress, anxiety, and lifestyle factors on the patient’s overall condition.
  
- **Action**: Recommends therapeutic approaches, stress-reduction strategies, or medication adjustments tailored to the patient’s psychological profile.

**3. Pulmonologist Agent**

- **Role**: Assess whether symptoms like shortness of breath and dizziness are due to a respiratory condition, such as asthma or a breathing disorder, that could mimic cardiac symptoms.
  
- **Action**: Suggests pulmonary function tests or other assessments and advises on treatments such as breathing exercises or medications when needed.

## Future Enhancements

In future versions, the system could expand to include a broader range of AI agents, each specializing in different medical fields, such as neurology, endocrinology, and immunology, to provide even more comprehensive analyses. These AI agents could be implemented using the [Assistant API from OpenAI](https://platform.openai.com/docs/assistants/overview) and use `function calling` and `code interpreter` capabilities to enhance their intelligence and effectiveness. Additionally, advanced parsing methodologies could be introduced to handle medical reports with more complex structures, allowing the system to accurately interpret and analyze a wider variety of medical data.

## Repository Structure

- **Medical Reports Folder**: Contains a synthetic medical report of a patient with Panic Attack disorder.
- **Results Folder**: Stores the outputs of the agentic system.
  
**To be able to run the code, please insert your OpenAI API key within the `apikey.env` file.**
